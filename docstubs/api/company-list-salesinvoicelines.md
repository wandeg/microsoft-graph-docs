---
title: "List salesInvoiceLines"
description: "Get the salesInvoiceLines from the salesInvoiceLines navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List salesInvoiceLines

Namespace: microsoft.graph

Get the salesInvoiceLines from the salesInvoiceLines navigation property.

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
GET /financials/companies/{companyId}/salesInvoiceLines
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
If successful, this method returns a `200 OK` response code and a collection of [salesInvoiceLine](../resources/salesinvoiceline.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salesinvoiceline"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesInvoiceLines
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.salesinvoiceline)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 992

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.salesInvoiceLine",
      "id": "e99f8ea7-8ea7-e99f-a78e-9fe9a78e9fe9",
      "documentId": "2cd4c5df-c5df-2cd4-dfc5-d42cdfc5d42c",
      "sequence": 8,
      "itemId": "38e36916-6916-38e3-1669-e3381669e338",
      "accountId": "7085e644-e644-7085-44e6-857044e68570",
      "lineType": "Line Type value",
      "description": "Description value",
      "unitOfMeasureId": "af6b7225-7225-af6b-2572-6baf25726baf",
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
  ]
}
```

