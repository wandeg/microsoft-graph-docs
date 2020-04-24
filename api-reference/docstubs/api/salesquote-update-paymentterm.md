---
title: "Update paymentTerm"
description: "Update the properties of a paymentTerm object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update paymentTerm

Namespace: microsoft.graph

Update the properties of a paymentTerm object.

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
PATCH /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/paymentTerm
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [paymentTerm](../resources/paymentterm.md) object.

The following table shows the properties that are required when you create the [paymentTerm](../resources/paymentterm.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|code|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|dueDateCalculation|String|**TODO: Add Description**|
|discountDateCalculation|String|**TODO: Add Description**|
|discountPercent|Decimal|**TODO: Add Description**|
|calculateDiscountOnCreditMemos|Boolean|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [paymentTerm](../resources/paymentterm.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_paymentterm"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/salesQuotes/{salesQuoteId}/paymentTerm
Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.paymentTerm",
  "id": "9cfce7bc-e7bc-9cfc-bce7-fc9cbce7fc9c",
  "code": "Code value",
  "displayName": "Display Name value",
  "dueDateCalculation": "Due Date Calculation value",
  "discountDateCalculation": "Discount Date Calculation value",
  "discountPercent": "4.2",
  "calculateDiscountOnCreditMemos": true,
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
}
```

