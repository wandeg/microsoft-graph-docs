---
title: "Create items"
description: "Create a new items object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create items

Namespace: microsoft.graph

Create a new items object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /connections/{connectionsId}/items
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [externalItem](../resources/externalitem.md) object.

The following table shows the properties that are required when you create the [externalItem](../resources/externalitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|properties|[properties](../resources/properties.md)|**TODO: Add Description**|
|content|[externalItemContent](../resources/externalitemcontent.md)|**TODO: Add Description**|
|acl|[acl](../resources/acl.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [externalItem](../resources/externalitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_externalitem_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/connections/{connectionsId}/items
Content-Type: application/json
Content-length: 284

{
  "@odata.type": "#microsoft.graph.externalItem",
  "properties": {
    "@odata.type": "microsoft.graph.properties"
  },
  "content": {
    "@odata.type": "microsoft.graph.externalItemContent"
  },
  "acl": [
    {
      "@odata.type": "microsoft.graph.acl"
    }
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalitem"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.externalItem",
  "id": "cad6d685-d685-cad6-85d6-d6ca85d6d6ca",
  "properties": {
    "@odata.type": "microsoft.graph.properties"
  },
  "content": {
    "@odata.type": "microsoft.graph.externalItemContent"
  },
  "acl": [
    {
      "@odata.type": "microsoft.graph.acl"
    }
  ]
}
```

