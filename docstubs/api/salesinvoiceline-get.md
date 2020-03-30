---
title: "Get salesInvoiceLine"
description: "Read properties and relationships of the salesInvoiceLine object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get salesInvoiceLine

Namespace: microsoft.graph

Read properties and relationships of the [salesInvoiceLine](../resources/salesinvoiceline.md) object.

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
GET /financials/companies/{companyId}/salesInvoiceLines/{salesInvoiceLineId}
GET /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/salesInvoiceLines/{salesInvoiceLineId}
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
If successful, this method returns a `200 OK` response code and [salesInvoiceLine](../resources/salesinvoiceline.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salesinvoiceline"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesInvoiceLines/{salesInvoiceLineId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesInvoiceLine"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 930

{
  "value": {
    "@odata.type": "#microsoft.graph.salesInvoiceLine",
    "id": "f4b3fe5c-fe5c-f4b3-5cfe-b3f45cfeb3f4",
    "documentId": "5bfe0542-0542-5bfe-4205-fe5b4205fe5b",
    "sequence": 8,
    "itemId": "33ceb353-b353-33ce-53b3-ce3353b3ce33",
    "accountId": "ec2602f3-02f3-ec26-f302-26ecf30226ec",
    "lineType": "Line Type value",
    "description": "Description value",
    "unitOfMeasureId": "dfeb54c9-54c9-dfeb-c954-ebdfc954ebdf",
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
}
```

