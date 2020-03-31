---
title: "Add salesInvoiceLines"
description: "Add salesInvoiceLines by posting to the salesInvoiceLines collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add salesInvoiceLines

Namespace: microsoft.graph

Add salesInvoiceLines by posting to the salesInvoiceLines collection.

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
POST /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/salesInvoiceLines/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [salesInvoiceLine](../resources/salesinvoiceline.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_salesinvoiceline_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/salesInvoiceLines
Content-type: application/json
Content-length: 814

{
  "@odata.type": "#microsoft.graph.salesInvoiceLine",
  "documentId": "80f7ddfe-ddfe-80f7-fedd-f780feddf780",
  "sequence": 8,
  "itemId": "5e7338b8-38b8-5e73-b838-735eb838735e",
  "accountId": "ca9f694c-694c-ca9f-4c69-9fca4c699fca",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "edff6ece-6ece-edff-ce6e-ffedce6effed",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.salesinvoiceline"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 863

{
  "@odata.type": "#microsoft.graph.salesInvoiceLine",
  "id": "01788e78-8e78-0178-788e-7801788e7801",
  "documentId": "80f7ddfe-ddfe-80f7-fedd-f780feddf780",
  "sequence": 8,
  "itemId": "5e7338b8-38b8-5e73-b838-735eb838735e",
  "accountId": "ca9f694c-694c-ca9f-4c69-9fca4c699fca",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "edff6ece-6ece-edff-ce6e-ffedce6effed",
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

