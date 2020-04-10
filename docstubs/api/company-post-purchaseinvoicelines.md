---
title: "Add purchaseInvoiceLines"
description: "Add purchaseInvoiceLines by posting to the purchaseInvoiceLines collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add purchaseInvoiceLines

Namespace: microsoft.graph

Add purchaseInvoiceLines by posting to the purchaseInvoiceLines collection.

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
POST /financials/companies/{companyId}/purchaseInvoiceLines/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [purchaseInvoiceLine](../resources/purchaseinvoiceline.md) object.

The following table shows the properties that are required when you create the [purchaseInvoiceLine](../resources/purchaseinvoiceline.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|documentId|Guid||
|sequence|Int32||
|itemId|Guid||
|accountId|Guid||
|lineType|String||
|description|String||
|unitCost|Decimal||
|quantity|Decimal||
|discountAmount|Decimal||
|discountPercent|Decimal||
|discountAppliedBeforeTax|Boolean||
|amountExcludingTax|Decimal||
|taxCode|String||
|taxPercent|Decimal||
|totalTaxAmount|Decimal||
|amountIncludingTax|Decimal||
|invoiceDiscountAllocation|Decimal||
|netAmount|Decimal||
|netTaxAmount|Decimal||
|netAmountIncludingTax|Decimal||
|expectedReceiptDate|Date||



## Response
If successful, this method returns a `201 Created` response code and a [purchaseInvoiceLine](../resources/purchaseinvoiceline.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_purchaseinvoiceline_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/purchaseInvoiceLines
Content-type: application/json
Content-length: 761

{
  "@odata.type": "#microsoft.graph.purchaseInvoiceLine",
  "documentId": "be260def-0def-be26-ef0d-26beef0d26be",
  "sequence": 8,
  "itemId": "f4d0acea-acea-f4d0-eaac-d0f4eaacd0f4",
  "accountId": "40910844-0844-4091-4408-914044089140",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitCost": "4.2",
  "quantity": "4.2",
  "discountAmount": "4.2",
  "discountPercent": "4.2",
  "discountAppliedBeforeTax": true,
  "amountExcludingTax": "4.2",
  "taxCode": "Tax Code value",
  "taxPercent": "4.2",
  "totalTaxAmount": "4.2",
  "amountIncludingTax": "4.2",
  "invoiceDiscountAllocation": "4.2",
  "netAmount": "4.2",
  "netTaxAmount": "4.2",
  "netAmountIncludingTax": "4.2",
  "expectedReceiptDate": "Date"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.purchaseinvoiceline"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 810

{
  "@odata.type": "#microsoft.graph.purchaseInvoiceLine",
  "id": "f7d7d579-d579-f7d7-79d5-d7f779d5d7f7",
  "documentId": "be260def-0def-be26-ef0d-26beef0d26be",
  "sequence": 8,
  "itemId": "f4d0acea-acea-f4d0-eaac-d0f4eaacd0f4",
  "accountId": "40910844-0844-4091-4408-914044089140",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitCost": "4.2",
  "quantity": "4.2",
  "discountAmount": "4.2",
  "discountPercent": "4.2",
  "discountAppliedBeforeTax": true,
  "amountExcludingTax": "4.2",
  "taxCode": "Tax Code value",
  "taxPercent": "4.2",
  "totalTaxAmount": "4.2",
  "amountIncludingTax": "4.2",
  "invoiceDiscountAllocation": "4.2",
  "netAmount": "4.2",
  "netTaxAmount": "4.2",
  "netAmountIncludingTax": "4.2",
  "expectedReceiptDate": "Date"
}
```

