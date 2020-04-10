---
title: "Get salesQuoteLine"
description: "Read properties and relationships of the salesQuoteLine object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get salesQuoteLine

Namespace: microsoft.graph

Read properties and relationships of the [salesQuoteLine](../resources/salesquoteline.md) object.

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
GET /financials/companies/{companyId}/salesQuoteLines/{salesQuoteLineId}
GET /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/salesQuoteLines/{salesQuoteLineId}
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
If successful, this method returns a `200 OK` response code and [salesQuoteLine](../resources/salesquoteline.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_salesquoteline"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesQuoteLines/{salesQuoteLineId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesQuoteLine"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 858

{
  "value": {
    "@odata.type": "#microsoft.graph.salesQuoteLine",
    "id": "c54bcd03-cd03-c54b-03cd-4bc503cd4bc5",
    "documentId": "be260def-0def-be26-ef0d-26beef0d26be",
    "sequence": 8,
    "itemId": "f4d0acea-acea-f4d0-eaac-d0f4eaacd0f4",
    "accountId": "40910844-0844-4091-4408-914044089140",
    "lineType": "Line Type value",
    "description": "Description value",
    "unitOfMeasureId": "7fef863c-863c-7fef-3c86-ef7f3c86ef7f",
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
    "netAmount": "4.2",
    "netTaxAmount": "4.2",
    "netAmountIncludingTax": "4.2"
  }
}
```

