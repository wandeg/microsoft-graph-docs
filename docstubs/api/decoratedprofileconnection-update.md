---
title: "Update DecoratedProfileConnection"
description: "Update the properties of a DecoratedProfileConnection object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update DecoratedProfileConnection

Namespace: microsoft.graph

Update the properties of a [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) object.

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
PATCH /decoratedProfileConnections/{decoratedProfileConnectionsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) object.

The following table shows the properties that are required when you create the [DecoratedProfileConnection](../resources/decoratedprofileconnection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|relevanceScore|Double||



## Response
If successful, this method returns a `200 OK` response code and an updated [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_decoratedprofileconnection"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/decoratedProfileConnections/{decoratedProfileConnectionsId}
Content-type: application/json
Content-length: 99

{
  "@odata.type": "#microsoft.graph.DecoratedProfileConnection",
  "relevanceScore": "Double"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 148

{
  "@odata.type": "#microsoft.graph.DecoratedProfileConnection",
  "id": "972173d1-73d1-9721-d173-2197d1732197",
  "relevanceScore": "Double"
}
```

