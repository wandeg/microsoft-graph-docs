---
title: "List items"
description: "Get the items from the items navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List items

Namespace: microsoft.graph

Get the items from the items navigation property.

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
GET /financials/companies/{companyId}/items
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [item](../resources/item.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_item"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/items
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.item)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 774

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.item",
      "id": "1c186fde-6fde-1c18-de6f-181cde6f181c",
      "number": "Number value",
      "displayName": "Display Name value",
      "type": "Type value",
      "itemCategoryId": "06d0fe0d-fe0d-06d0-0dfe-d0060dfed006",
      "itemCategoryCode": "Item Category Code value",
      "blocked": true,
      "baseUnitOfMeasureId": "3f0cfef8-fef8-3f0c-f8fe-0c3ff8fe0c3f",
      "gtin": "Gtin value",
      "inventory": "4.2",
      "unitPrice": "4.2",
      "priceIncludesTax": true,
      "unitCost": "4.2",
      "taxGroupId": "0641b09e-b09e-0641-9eb0-41069eb04106",
      "taxGroupCode": "Tax Group Code value",
      "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00"
    }
  ]
}
```

