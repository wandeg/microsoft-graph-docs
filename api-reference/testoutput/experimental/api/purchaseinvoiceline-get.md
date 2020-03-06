---
title: "Get purchaseInvoiceLine"
description: "Read properties and relationships of the purchaseInvoiceLine object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get purchaseInvoiceLine

Namespace: microsoft.graph

Read properties and relationships of the [purchaseInvoiceLine](../resources/purchaseinvoiceline.md) object.

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
GET /financials/companies/{companyId}/purchaseInvoiceLines/{purchaseInvoiceLineId}
GET /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}/purchaseInvoiceLines/{purchaseInvoiceLineId}
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
If successful, this method returns a `200 OK` response code and [purchaseInvoiceLine](../resources/purchaseinvoiceline.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_purchaseinvoiceline"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/purchaseInvoiceLines/{purchaseInvoiceLineId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.purchaseInvoiceLine"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 875

{
  "value": {
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
}
```

