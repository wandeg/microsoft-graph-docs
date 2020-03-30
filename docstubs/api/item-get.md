---
title: "Get item"
description: "Read properties and relationships of the item object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get item

Namespace: microsoft.graph

Read properties and relationships of the [item](../resources/item.md) object.

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
GET /financials/companies/{companyId}/items/{itemId}
GET /financials/companies/{companyId}/salesOrders/{salesOrderId}/salesOrderLines/{salesOrderLineId}/item
GET /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/salesQuoteLines/{salesQuoteLineId}/item
GET /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/salesInvoiceLines/{salesInvoiceLineId}/item
GET /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/salesCreditMemoLines/{salesCreditMemoLineId}/item
GET /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}/purchaseInvoiceLines/{purchaseInvoiceLineId}/item
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
If successful, this method returns a `200 OK` response code and [item](../resources/item.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_item"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/items/{itemId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.item"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 726

{
  "value": {
    "@odata.type": "#microsoft.graph.item",
    "id": "ca07066a-066a-ca07-6a06-07ca6a0607ca",
    "number": "Number value",
    "displayName": "Display Name value",
    "type": "Type value",
    "itemCategoryId": "3ce86479-6479-3ce8-7964-e83c7964e83c",
    "itemCategoryCode": "Item Category Code value",
    "blocked": true,
    "baseUnitOfMeasureId": "443c57c7-57c7-443c-c757-3c44c7573c44",
    "gtin": "Gtin value",
    "inventory": "4.2",
    "unitPrice": "4.2",
    "priceIncludesTax": true,
    "unitCost": "4.2",
    "taxGroupId": "38fa40bf-40bf-38fa-bf40-fa38bf40fa38",
    "taxGroupCode": "Tax Group Code value",
    "lastModifiedDateTime": "2017-01-01T00:02:50.3839766+00:00"
  }
}
```

