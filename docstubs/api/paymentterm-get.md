---
title: "Get paymentTerm"
description: "Read properties and relationships of the paymentTerm object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get paymentTerm

Namespace: microsoft.graph

Read properties and relationships of the [paymentTerm](../resources/paymentterm.md) object.

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
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [paymentTerm](../resources/paymentterm.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_paymentterm"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/paymentTerms/{paymentTermId}
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
    "id": "261d619a-619a-261d-9a61-1d269a611d26",
    "code": "Code value",
    "displayName": "Display Name value",
    "dueDateCalculation": "Due Date Calculation value",
    "discountDateCalculation": "Discount Date Calculation value",
    "discountPercent": "4.2",
    "calculateDiscountOnCreditMemos": true,
    "lastModifiedDateTime": "2017-01-01T00:01:52.9217945+03:00"
  }
}
```

