---
title: "Create audioRoutingGroup"
description: "Create a new audioRoutingGroup object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create audioRoutingGroup

Namespace: microsoft.graph

Create a new [audioRoutingGroup](../resources/audioroutinggroup.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /communications/calls/{callId}/audioRoutingGroups
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [audioRoutingGroup](../resources/audioroutinggroup.md) object.

The following table shows the properties that are required when you create the [audioRoutingGroup](../resources/audioroutinggroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|routingMode|Enumeration|. Possible values are: `oneToOne`, `multicast`.|
|sources|String collection||
|receivers|String collection||



## Response
If successful, this method returns a `201 Created` response code and a [audioRoutingGroup](../resources/audioroutinggroup.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_audioroutinggroup_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/communications/calls/{callId}/audioRoutingGroups
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
  "truncated": true,
  "@odata.type": "microsoft.graph.audioroutinggroup"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 226

{
  "@odata.type": "#microsoft.graph.audioRoutingGroup",
  "id": "af751337-1337-af75-3713-75af371375af",
  "routingMode": "String",
  "sources": [
    "Sources value"
  ],
  "receivers": [
    "Receivers value"
  ]
}
```

