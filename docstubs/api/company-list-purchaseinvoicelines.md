---
title: "List purchaseInvoiceLines"
description: "Get the purchaseInvoiceLines from the purchaseInvoiceLines navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List purchaseInvoiceLines

Namespace: microsoft.graph

Get the purchaseInvoiceLines from the purchaseInvoiceLines navigation property.

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
GET /financials/companies/{companyId}/purchaseInvoiceLines
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [purchaseInvoiceLine](../resources/purchaseinvoiceline.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_purchaseinvoiceline"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/purchaseInvoiceLines
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.purchaseinvoiceline)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 935

{
  "value": [
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
  ]
}
```

