---
title: "List items"
description: "Get the externalItems from the items navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List items

Namespace: microsoft.graph

Get the externalItems from the items navigation property.

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
GET /connections/{connectionsId}/items
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [externalItem](../resources/externalitem.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_externalitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/connections/{connectionsId}/items
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.externalitem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

