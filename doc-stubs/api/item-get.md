---
title: "Get item"
description: "Read the properties and relationships of an item object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get item

Namespace: microsoft.graph

Read the properties and relationships of an [item](../resources/item.md) object.

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
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [item](../resources/item.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_item"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/items/{itemId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.item"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.item",
    "id": "0559707c-707c-0559-7c70-59057c705905",
    "number": "String",
    "displayName": "String",
    "type": "String",
    "itemCategoryId": "Guid",
    "itemCategoryCode": "String",
    "blocked": "Boolean",
    "baseUnitOfMeasureId": "Guid",
    "gtin": "String",
    "inventory": "Decimal",
    "unitPrice": "Decimal",
    "priceIncludesTax": "Boolean",
    "unitCost": "Decimal",
    "taxGroupId": "Guid",
    "taxGroupCode": "String",
    "lastModifiedDateTime": "String (timestamp)"
  }
}
```

