---
title: "Update paymentTerm"
description: "Update the properties of a paymentTerm object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update paymentTerm

Namespace: microsoft.graph

Update the properties of a [paymentTerm](../resources/paymentterm.md) object.

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
PATCH /financials/companies/{companyId}/paymentTerms/{paymentTermId}
PATCH /financials/companies/{companyId}/vendors/{vendorId}/paymentTerm
PATCH /financials/companies/{companyId}/customers/{customerId}/paymentTerm
PATCH /financials/companies/{companyId}/salesOrders/{salesOrderId}/paymentTerm
PATCH /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/paymentTerm
PATCH /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/paymentTerm
PATCH /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/paymentTerm
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [paymentTerm](../resources/paymentterm.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_paymentterm"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/paymentTerms/{paymentTermId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 423

{
  "@odata.type": "#microsoft.graph.paymentTerm",
  "id": "bae6edca-edca-bae6-caed-e6bacaede6ba",
  "code": "Code value",
  "displayName": "Display Name value",
  "dueDateCalculation": "Due Date Calculation value",
  "discountDateCalculation": "Discount Date Calculation value",
  "discountPercent": "4.2",
  "calculateDiscountOnCreditMemos": true,
  "lastModifiedDateTime": "2017-01-01T00:02:50.3839766+00:00"
}
```

