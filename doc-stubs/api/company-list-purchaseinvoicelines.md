---
title: "List purchaseInvoiceLines"
description: "Get the purchaseInvoiceLines from the purchaseInvoiceLines navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List purchaseInvoiceLines

Namespace: microsoft.graph

Get the purchaseInvoiceLines from the purchaseInvoiceLines navigation property.

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
GET /financials/companies/{companyId}/purchaseInvoiceLines
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.purchaseinvoiceline)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.purchaseInvoiceLine",
      "id": "7a9c9a6c-9a6c-7a9c-6c9a-9c7a6c9a9c7a",
      "documentId": "Guid",
      "sequence": "Integer",
      "itemId": "Guid",
      "accountId": "Guid",
      "lineType": "String",
      "description": "String",
      "unitCost": "Decimal",
      "quantity": "Decimal",
      "discountAmount": "Decimal",
      "discountPercent": "Decimal",
      "discountAppliedBeforeTax": "Boolean",
      "amountExcludingTax": "Decimal",
      "taxCode": "String",
      "taxPercent": "Decimal",
      "totalTaxAmount": "Decimal",
      "amountIncludingTax": "Decimal",
      "invoiceDiscountAllocation": "Decimal",
      "netAmount": "Decimal",
      "netTaxAmount": "Decimal",
      "netAmountIncludingTax": "Decimal",
      "expectedReceiptDate": "Date"
    }
  ]
}
```

