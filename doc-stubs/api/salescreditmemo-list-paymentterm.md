---
title: "List paymentTerm"
description: "Get the paymentTerms from the paymentTerm navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List paymentTerm

Namespace: microsoft.graph

Get the paymentTerms from the paymentTerm navigation property.

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
GET /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/paymentTerm
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

If successful, this method returns a `200 OK` response code and a collection of [paymentTerm](../resources/paymentterm.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_paymentterm"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/paymentTerm
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.paymentterm)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.paymentTerm",
      "id": "e3b2579f-579f-e3b2-9f57-b2e39f57b2e3",
      "code": "String",
      "displayName": "String",
      "dueDateCalculation": "String",
      "discountDateCalculation": "String",
      "discountPercent": "Decimal",
      "calculateDiscountOnCreditMemos": "Boolean",
      "lastModifiedDateTime": "String (timestamp)"
    }
  ]
}
```

