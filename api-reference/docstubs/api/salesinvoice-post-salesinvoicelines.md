---
title: "Create salesInvoiceLines"
description: "Create a new salesInvoiceLines object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create salesInvoiceLines

Namespace: microsoft.graph

Create a new salesInvoiceLines object.

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
POST /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/salesInvoiceLines
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [salesInvoiceLine](../resources/salesinvoiceline.md) object.

The following table shows the properties that are required when you create the [salesInvoiceLine](../resources/salesinvoiceline.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|documentId|Guid|**TODO: Add Description**|
|sequence|Int32|**TODO: Add Description**|
|itemId|Guid|**TODO: Add Description**|
|accountId|Guid|**TODO: Add Description**|
|lineType|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|unitOfMeasureId|Guid|**TODO: Add Description**|
|unitPrice|Decimal|**TODO: Add Description**|
|quantity|Decimal|**TODO: Add Description**|
|discountAmount|Decimal|**TODO: Add Description**|
|discountPercent|Decimal|**TODO: Add Description**|
|discountAppliedBeforeTax|Boolean|**TODO: Add Description**|
|amountExcludingTax|Decimal|**TODO: Add Description**|
|taxCode|String|**TODO: Add Description**|
|taxPercent|Decimal|**TODO: Add Description**|
|totalTaxAmount|Decimal|**TODO: Add Description**|
|amountIncludingTax|Decimal|**TODO: Add Description**|
|invoiceDiscountAllocation|Decimal|**TODO: Add Description**|
|netAmount|Decimal|**TODO: Add Description**|
|netTaxAmount|Decimal|**TODO: Add Description**|
|netAmountIncludingTax|Decimal|**TODO: Add Description**|
|shipmentDate|Date|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [salesInvoiceLine](../resources/salesinvoiceline.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_salesinvoiceline_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/salesInvoiceLines
Content-Type: application/json
Content-length: 814

{
  "@odata.type": "#microsoft.graph.salesInvoiceLine",
  "documentId": "165821c2-21c2-1658-c221-5816c2215816",
  "sequence": 8,
  "itemId": "4443d486-d486-4443-86d4-434486d44344",
  "accountId": "157ed6fe-d6fe-157e-fed6-7e15fed67e15",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "d75c434a-434a-d75c-4a43-5cd74a435cd7",
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesinvoiceline"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.salesInvoiceLine",
  "id": "288fa36b-a36b-288f-6ba3-8f286ba38f28",
  "documentId": "165821c2-21c2-1658-c221-5816c2215816",
  "sequence": 8,
  "itemId": "4443d486-d486-4443-86d4-434486d44344",
  "accountId": "157ed6fe-d6fe-157e-fed6-7e15fed67e15",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "d75c434a-434a-d75c-4a43-5cd74a435cd7",
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

