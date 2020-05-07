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
|Authorization|Bearer {token}. Required.|

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
    "id": "90d7ea88-ea88-90d7-88ea-d79088ead790",
    "documentId": "Guid",
    "sequence": "Integer",
    "itemId": "Guid",
    "accountId": "Guid",
    "lineType": "String",
    "description": "String",
    "unitOfMeasureId": "Guid",
    "unitPrice": "Decimal",
    "quantity": "Decimal",
    "discountAmount": "Decimal",
    "discountPercent": "Decimal",
    "discountAppliedBeforeTax": "Boolean",
    "amountExcludingTax": "Decimal",
    "taxCode": "String",
    "taxPercent": "Decimal",
    "totalTaxAmount": "Decimal",
    "amountIncludingTax": "Decimal",
    "netAmount": "Decimal",
    "netTaxAmount": "Decimal",
    "netAmountIncludingTax": "Decimal"
  }
}
```

