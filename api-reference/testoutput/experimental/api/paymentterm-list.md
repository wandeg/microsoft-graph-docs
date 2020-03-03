---
title: "List paymentTerms"
description: "List properties and relationships of the paymentTerm objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List paymentTerms

Namespace: microsoft.graph

List properties and relationships of the [paymentTerm](../resources/paymentterm.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /financials/companies/{companyId}/paymentTerms
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [paymentTerm](../resources/paymentterm.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_paymentterm"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/paymentTerms
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
      "id": "2c9c3f95-3f95-2c9c-953f-9c2c953f9c2c",
      "code": "Code value",
      "displayName": "Display Name value",
      "dueDateCalculation": "Due Date Calculation value",
      "discountDateCalculation": "Discount Date Calculation value",
      "discountPercent": "4.2",
      "calculateDiscountOnCreditMemos": true,
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00"
    }
  ]
}
```

