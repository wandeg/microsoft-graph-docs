---
title: "List paymentTerms"
description: "Get the paymentTerms from the paymentTerms navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List paymentTerms

Namespace: microsoft.graph

Get the paymentTerms from the paymentTerms navigation property.

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
GET /financials/companies/{companyId}/paymentTerms
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
If successful, this method returns a `200 OK` response code and a collection of [paymentTerm](../resources/paymentterm.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_paymentterm"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/paymentTerms
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.paymentterm)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 492

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.paymentTerm",
      "id": "67a4113b-113b-67a4-3b11-a4673b11a467",
      "code": "Code value",
      "displayName": "Display Name value",
      "dueDateCalculation": "Due Date Calculation value",
      "discountDateCalculation": "Discount Date Calculation value",
      "discountPercent": "4.2",
      "calculateDiscountOnCreditMemos": true,
      "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00"
    }
  ]
}
```

