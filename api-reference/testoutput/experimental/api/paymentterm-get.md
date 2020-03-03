---
title: "Get paymentTerm"
description: "Read properties and relationships of the paymentTerm object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get paymentTerm

Read properties and relationships of the [paymentTerm](../resources/paymentterm.md) object.

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
GET /financials/companies/{companyId}/paymentTerms/{paymentTermId}
GET /financials/companies/{companyId}/vendors/{vendorId}/paymentTerm
GET /financials/companies/{companyId}/customers/{customerId}/paymentTerm
GET /financials/companies/{companyId}/salesOrders/{salesOrderId}/paymentTerm
GET /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/paymentTerm
GET /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/paymentTerm
GET /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/paymentTerm
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [paymentTerm](../resources/paymentterm.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_paymentterm"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/financials/companies/{companyId}/paymentTerms/{paymentTermId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.paymentTerm"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 460

{
  "value": {
    "@odata.type": "#microsoft.graph.paymentTerm",
    "id": "c6215f36-5f36-c621-365f-21c6365f21c6",
    "code": "Code value",
    "displayName": "Display Name value",
    "dueDateCalculation": "Due Date Calculation value",
    "discountDateCalculation": "Discount Date Calculation value",
    "discountPercent": "4.2",
    "calculateDiscountOnCreditMemos": true,
    "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00"
  }
}
```

