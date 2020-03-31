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
|Name|Description|
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
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesQuotes/{salesQuoteId}/salesQuoteLines
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
      "id": "b82de450-e450-b82d-50e4-2db850e42db8",
      "documentId": "a96669d7-69d7-a966-d769-66a9d76966a9",
      "sequence": 8,
      "itemId": "aefdf05f-f05f-aefd-5ff0-fdae5ff0fdae",
      "accountId": "ecadd616-d616-ecad-16d6-adec16d6adec",
      "lineType": "Line Type value",
      "description": "Description value",
      "unitOfMeasureId": "9f28e186-e186-9f28-86e1-289f86e1289f",
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

