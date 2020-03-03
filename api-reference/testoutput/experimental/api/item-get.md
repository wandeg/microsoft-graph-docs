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

## HTTP Request
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
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [item](../resources/item.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_item"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/items/{itemId}
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
    "id": "18a35fd7-5fd7-18a3-d75f-a318d75fa318",
    "number": "Number value",
    "displayName": "Display Name value",
    "type": "Type value",
    "itemCategoryId": "f6c1027d-027d-f6c1-7d02-c1f67d02c1f6",
    "itemCategoryCode": "Item Category Code value",
    "blocked": true,
    "baseUnitOfMeasureId": "33eceb10-eb10-33ec-10eb-ec3310ebec33",
    "gtin": "Gtin value",
    "inventory": "4.2",
    "unitPrice": "4.2",
    "priceIncludesTax": true,
    "unitCost": "4.2",
    "taxGroupId": "d4a99fdf-9fdf-d4a9-df9f-a9d4df9fa9d4",
    "taxGroupCode": "Tax Group Code value",
    "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00"
  }
}
```

