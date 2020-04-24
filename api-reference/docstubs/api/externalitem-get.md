---
title: "Get externalItem"
description: "Read the properties and relationships of an externalItem object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get externalItem

Namespace: microsoft.graph

Read the properties and relationships of an [externalItem](../resources/externalitem.md) object.

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
GET /connections/{connectionsId}/items/{externalItemId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and an [externalItem](../resources/externalitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_externalitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/connections/{connectionsId}/items/{externalItemId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.externalItem",
    "id": "77e6c19a-c19a-77e6-9ac1-e6779ac1e677",
    "properties": {
      "@odata.type": "microsoft.graph.properties"
    },
    "content": {
      "@odata.type": "microsoft.graph.externalItemContent",
      "value": "Value value",
      "type": "String"
    },
    "acl": [
      {
        "@odata.type": "microsoft.graph.acl",
        "type": "String",
        "accessType": "String",
        "identitySource": "Identity Source value"
      }
    ]
  }
}
```

