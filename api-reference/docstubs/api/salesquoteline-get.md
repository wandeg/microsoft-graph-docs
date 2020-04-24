---
title: "Get salesQuoteLine"
description: "Read the properties and relationships of a salesQuoteLine object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get salesQuoteLine

Namespace: microsoft.graph

Read the properties and relationships of a [salesQuoteLine](../resources/salesquoteline.md) object.

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
GET /financials/companies/{companyId}/salesQuoteLines/{salesQuoteLineId}
GET /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/salesQuoteLines/{salesQuoteLineId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [salesQuoteLine](../resources/salesquoteline.md) object in the response body.

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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesQuoteLine"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.salesQuoteLine",
    "id": "65e90600-0600-65e9-0006-e9650006e965",
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
    "netAmount": "4.2",
    "netTaxAmount": "4.2",
    "netAmountIncludingTax": "4.2"
  }
}
```

