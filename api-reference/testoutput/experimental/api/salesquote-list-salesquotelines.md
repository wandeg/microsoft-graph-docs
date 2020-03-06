---
title: "List salesQuoteLines"
description: "Get the salesQuoteLines from the salesQuoteLines navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List salesQuoteLines

Namespace: microsoft.graph

Get the salesQuoteLines from the salesQuoteLines navigation property.

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
GET /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/salesQuoteLines
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
If successful, this method returns a `200 OK` response code and a collection of [salesQuoteLine](../resources/salesquoteline.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salesquoteline"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/salesQuotes/{salesQuoteId}/salesQuoteLines
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.salesquoteline)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 916

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.salesQuoteLine",
      "id": "cd74ed39-ed39-cd74-39ed-74cd39ed74cd",
      "documentId": "f25796de-96de-f257-de96-57f2de9657f2",
      "sequence": 8,
      "itemId": "39a5aaf7-aaf7-39a5-f7aa-a539f7aaa539",
      "accountId": "16975858-5858-1697-5858-971658589716",
      "lineType": "Line Type value",
      "description": "Description value",
      "unitOfMeasureId": "8736d1fa-d1fa-8736-fad1-3687fad13687",
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
  ]
}
```

