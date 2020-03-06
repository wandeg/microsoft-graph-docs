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
|Header|Value|
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
    "id": "5e2b48a8-48a8-5e2b-a848-2b5ea8482b5e",
    "number": "Number value",
    "displayName": "Display Name value",
    "type": "Type value",
    "itemCategoryId": "35a8b44c-b44c-35a8-4cb4-a8354cb4a835",
    "itemCategoryCode": "Item Category Code value",
    "blocked": true,
    "baseUnitOfMeasureId": "ec01bd51-bd51-ec01-51bd-01ec51bd01ec",
    "gtin": "Gtin value",
    "inventory": "4.2",
    "unitPrice": "4.2",
    "priceIncludesTax": true,
    "unitCost": "4.2",
    "taxGroupId": "46cf8feb-8feb-46cf-eb8f-cf46eb8fcf46",
    "taxGroupCode": "Tax Group Code value",
    "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00"
  }
}
```

