---
title: "Update purchaseInvoiceLine"
description: "Update the properties of a purchaseInvoiceLine object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update purchaseInvoiceLine

Namespace: microsoft.graph

Update the properties of a [purchaseInvoiceLine](../resources/purchaseinvoiceline.md) object.

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
PATCH /financials/companies/{companyId}/purchaseInvoiceLines/{purchaseInvoiceLineId}
PATCH /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}/purchaseInvoiceLines/{purchaseInvoiceLineId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [purchaseInvoiceLine](../resources/purchaseinvoiceline.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_purchaseinvoiceline"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/financials/companies/{companyId}/purchaseInvoiceLines/{purchaseInvoiceLineId}
Content-type: application/json
Content-length: 761

{
  "@odata.type": "#microsoft.graph.purchaseInvoiceLine",
  "documentId": "f25796de-96de-f257-de96-57f2de9657f2",
  "sequence": 8,
  "itemId": "39a5aaf7-aaf7-39a5-f7aa-a539f7aaa539",
  "accountId": "16975858-5858-1697-5858-971658589716",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 810

{
  "@odata.type": "#microsoft.graph.purchaseInvoiceLine",
  "id": "e1ced5a7-d5a7-e1ce-a7d5-cee1a7d5cee1",
  "documentId": "f25796de-96de-f257-de96-57f2de9657f2",
  "sequence": 8,
  "itemId": "39a5aaf7-aaf7-39a5-f7aa-a539f7aaa539",
  "accountId": "16975858-5858-1697-5858-971658589716",
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

