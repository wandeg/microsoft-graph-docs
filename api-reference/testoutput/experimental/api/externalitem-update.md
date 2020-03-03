---
title: "Update externalItem"
description: "Update the properties of a externalItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update externalItem

Update the properties of a [externalItem](../resources/externalitem.md) object.

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
PATCH /connections/{connectionsId}/items/{externalItemId}
PATCH /external/connections/{externalConnectionId}/items/{externalItemId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [externalItem](../resources/externalItem.md) object.

The following table shows the properties that are required when you create the [externalItem](../resources/externalitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|properties|[properties](../resources/properties.md)||
|content|String||
|acl|[acl](../resources/acl.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [externalItem](../resources/externalitem.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_externalitem"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/connections/{connectionsId}/items/{externalItemId}
Content-type: application/json
Content-length: 372

{
  "@odata.type": "#microsoft.graph.externalItem",
  "properties": {
    "@odata.type": "microsoft.graph.properties"
  },
  "content": "Content value",
  "acl": [
    {
      "@odata.type": "microsoft.graph.acl",
      "type": "String",
      "value": "Value value",
      "accessType": "String",
      "identitySource": "Identity Source value"
    }
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
Content-Length: 421

{
  "@odata.type": "#microsoft.graph.externalItem",
  "id": "e4ac5c1d-5c1d-e4ac-1d5c-ace41d5cace4",
  "properties": {
    "@odata.type": "microsoft.graph.properties"
  },
  "content": "Content value",
  "acl": [
    {
      "@odata.type": "microsoft.graph.acl",
      "type": "String",
      "value": "Value value",
      "accessType": "String",
      "identitySource": "Identity Source value"
    }
  ]
}
```

