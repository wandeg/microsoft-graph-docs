---
title: "Add items"
description: "Add items by posting to the items collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add items

Namespace: microsoft.graph

Add items by posting to the items collection.

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
POST /connections/{connectionsId}/items/$ref
POST /external/connections/{externalConnectionId}/items/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [externalItem](../resources/externalitem.md) object.

The following table shows the properties that are required when you create the [externalItem](../resources/externalitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|properties|[properties](../resources/properties.md)||
|content|String||
|acl|[acl](../resources/acl.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [externalItem](../resources/externalitem.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/connections/{connectionsId}/items
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
  "truncated": true,
  "@odata.type": "microsoft.graph.externalitem"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 421

{
  "@odata.type": "#microsoft.graph.externalItem",
  "id": "6480ebb0-ebb0-6480-b0eb-8064b0eb8064",
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

