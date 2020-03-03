---
title: "Add paymentTerms"
description: "Add paymentTerms by posting to the paymentTerms collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add paymentTerms

Namespace: microsoft.graph

Add paymentTerms by posting to the paymentTerms collection.

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
POST /financials/companies/{companyId}/paymentTerms/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [paymentTerm](../resources/paymentterm.md) object.

The following table shows the properties that are required when you create the [paymentTerm](../resources/paymentterm.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|code|String||
|displayName|String||
|dueDateCalculation|String||
|discountDateCalculation|String||
|discountPercent|Decimal||
|calculateDiscountOnCreditMemos|Boolean||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [paymentTerm](../resources/paymentterm.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_paymentterm_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/financials/companies/{companyId}/paymentTerms
Content-type: application/json
Content-length: 310

{
  "@odata.type": "#microsoft.graph.paymentTerm",
  "code": "Code value",
  "displayName": "Display Name value",
  "dueDateCalculation": "Due Date Calculation value",
  "discountDateCalculation": "Discount Date Calculation value",
  "discountPercent": "4.2",
  "calculateDiscountOnCreditMemos": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.paymentterm"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 423

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
```

