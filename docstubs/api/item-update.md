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
Here is an example of the request.
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
  "itemCategoryId": "2f905af9-5af9-2f90-f95a-902ff95a902f",
  "itemCategoryCode": "Item Category Code value",
  "blocked": true,
  "baseUnitOfMeasureId": "c4a55195-5195-c4a5-9551-a5c49551a5c4",
  "gtin": "Gtin value",
  "inventory": "4.2",
  "unitPrice": "4.2",
  "priceIncludesTax": true,
  "unitCost": "4.2",
  "taxGroupId": "1be4f5fb-f5fb-1be4-fbf5-e41bfbf5e41b",
  "taxGroupCode": "Tax Group Code value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
  "id": "d9f47e77-7e77-d9f4-777e-f4d9777ef4d9",
  "number": "Number value",
  "displayName": "Display Name value",
  "type": "Type value",
  "itemCategoryId": "2f905af9-5af9-2f90-f95a-902ff95a902f",
  "itemCategoryCode": "Item Category Code value",
  "blocked": true,
  "baseUnitOfMeasureId": "c4a55195-5195-c4a5-9551-a5c49551a5c4",
  "gtin": "Gtin value",
  "inventory": "4.2",
  "unitPrice": "4.2",
  "priceIncludesTax": true,
  "unitCost": "4.2",
  "taxGroupId": "1be4f5fb-f5fb-1be4-fbf5-e41bfbf5e41b",
  "taxGroupCode": "Tax Group Code value",
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00"
}
```

