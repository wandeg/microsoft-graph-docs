---
title: "Update audioRoutingGroup"
description: "Update the properties of a audioRoutingGroup object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update audioRoutingGroup

Namespace: microsoft.graph

Update the properties of a [audioRoutingGroup](../resources/audioroutinggroup.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /app/calls/{callId}/audioRoutingGroups/{audioRoutingGroupId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [audioRoutingGroup](../resources/audioroutinggroup.md) object.

The following table shows the properties that are required when you create the [audioRoutingGroup](../resources/audioroutinggroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|routingMode|Enumeration| Possible values are: `oneToOne`, `multicast`.|
|sources|String collection||
|receivers|String collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_audioroutinggroup"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/app/calls/{callId}/audioRoutingGroups/{audioRoutingGroupId}
Content-type: application/json
Content-length: 177

{
  "@odata.type": "#microsoft.graph.audioRoutingGroup",
  "routingMode": "String",
  "sources": [
    "Sources value"
  ],
  "receivers": [
    "Receivers value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 226

{
  "@odata.type": "#microsoft.graph.audioRoutingGroup",
  "id": "d309a6ff-a6ff-d309-ffa6-09d3ffa609d3",
  "routingMode": "String",
  "sources": [
    "Sources value"
  ],
  "receivers": [
    "Receivers value"
  ]
}
```

