---
title: "Update item"
description: "Update the properties of a item object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update item

Namespace: microsoft.graph

Update the properties of a [item](../resources/item.md) object.

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
PATCH /financials/companies/{companyId}/items/{itemId}
PATCH /financials/companies/{companyId}/salesOrders/{salesOrderId}/salesOrderLines/{salesOrderLineId}/item
PATCH /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/salesQuoteLines/{salesQuoteLineId}/item
PATCH /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/salesInvoiceLines/{salesInvoiceLineId}/item
PATCH /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/salesCreditMemoLines/{salesCreditMemoLineId}/item
PATCH /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}/purchaseInvoiceLines/{purchaseInvoiceLineId}/item
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [item](../resources/item.md) object.

The following table shows the properties that are required when you create the [item](../resources/item.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|number|String||
|displayName|String||
|type|String||
|itemCategoryId|Guid||
|itemCategoryCode|String||
|blocked|Boolean||
|baseUnitOfMeasureId|Guid||
|gtin|String||
|inventory|Decimal||
|unitPrice|Decimal||
|priceIncludesTax|Boolean||
|unitCost|Decimal||
|taxGroupId|Guid||
|taxGroupCode|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [item](../resources/item.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_item"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/items/{itemId}
Content-type: application/json
Content-length: 560

{
  "@odata.type": "#microsoft.graph.item",
  "number": "Number value",
  "displayName": "Display Name value",
  "type": "Type value",
  "itemCategoryId": "7bf434a3-34a3-7bf4-a334-f47ba334f47b",
  "itemCategoryCode": "Item Category Code value",
  "blocked": true,
  "baseUnitOfMeasureId": "83bf0936-0936-83bf-3609-bf833609bf83",
  "gtin": "Gtin value",
  "inventory": "4.2",
  "unitPrice": "4.2",
  "priceIncludesTax": true,
  "unitCost": "4.2",
  "taxGroupId": "1245f020-f020-1245-20f0-451220f04512",
  "taxGroupCode": "Tax Group Code value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 673

{
  "@odata.type": "#microsoft.graph.item",
  "id": "0106eaeb-eaeb-0106-ebea-0601ebea0601",
  "number": "Number value",
  "displayName": "Display Name value",
  "type": "Type value",
  "itemCategoryId": "7bf434a3-34a3-7bf4-a334-f47ba334f47b",
  "itemCategoryCode": "Item Category Code value",
  "blocked": true,
  "baseUnitOfMeasureId": "83bf0936-0936-83bf-3609-bf833609bf83",
  "gtin": "Gtin value",
  "inventory": "4.2",
  "unitPrice": "4.2",
  "priceIncludesTax": true,
  "unitCost": "4.2",
  "taxGroupId": "1245f020-f020-1245-20f0-451220f04512",
  "taxGroupCode": "Tax Group Code value",
  "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00"
}
```

