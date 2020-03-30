---
title: "Update salesInvoiceLine"
description: "Update the properties of a salesInvoiceLine object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update salesInvoiceLine

Namespace: microsoft.graph

Update the properties of a [salesInvoiceLine](../resources/salesinvoiceline.md) object.

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
PATCH /financials/companies/{companyId}/salesInvoiceLines/{salesInvoiceLineId}
PATCH /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/salesInvoiceLines/{salesInvoiceLineId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [salesInvoiceLine](../resources/salesinvoiceline.md) object.

The following table shows the properties that are required when you create the [salesInvoiceLine](../resources/salesinvoiceline.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|documentId|Guid||
|sequence|Int32||
|itemId|Guid||
|accountId|Guid||
|lineType|String||
|description|String||
|unitOfMeasureId|Guid||
|unitPrice|Decimal||
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
|shipmentDate|Date||



## Response
If successful, this method returns a `200 OK` response code and an updated [salesInvoiceLine](../resources/salesinvoiceline.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_salesinvoiceline"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/salesInvoiceLines/{salesInvoiceLineId}
Content-type: application/json
Content-length: 814

{
  "@odata.type": "#microsoft.graph.salesInvoiceLine",
  "documentId": "ad0679c0-79c0-ad06-c079-06adc07906ad",
  "sequence": 8,
  "itemId": "b63d2521-2521-b63d-2125-3db621253db6",
  "accountId": "93d19a1f-9a1f-93d1-1f9a-d1931f9ad193",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "e854acc8-acc8-e854-c8ac-54e8c8ac54e8",
  "unitPrice": "4.2",
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
  "shipmentDate": "Date"
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
Content-Length: 863

{
  "@odata.type": "#microsoft.graph.salesInvoiceLine",
  "id": "66053e7f-3e7f-6605-7f3e-05667f3e0566",
  "documentId": "ad0679c0-79c0-ad06-c079-06adc07906ad",
  "sequence": 8,
  "itemId": "b63d2521-2521-b63d-2125-3db621253db6",
  "accountId": "93d19a1f-9a1f-93d1-1f9a-d1931f9ad193",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "e854acc8-acc8-e854-c8ac-54e8c8ac54e8",
  "unitPrice": "4.2",
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
  "shipmentDate": "Date"
}
```

