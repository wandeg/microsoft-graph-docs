---
title: "Get customer"
description: "Read properties and relationships of the customer object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get customer

Namespace: microsoft.graph

Read properties and relationships of the [customer](../resources/customer.md) object.

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
GET /financials/companies/{companyId}/customers/{customerId}
GET /financials/companies/{companyId}/salesOrders/{salesOrderId}/customer
GET /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/customer
GET /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/customer
GET /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/customer
GET /financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}/customerPayments/{customerPaymentId}/customer
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [customer](../resources/customer.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_customer"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/customers/{customerId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customer"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1199

{
  "value": {
    "@odata.type": "#microsoft.graph.customer",
    "id": "c5bc16d9-16d9-c5bc-d916-bcc5d916bcc5",
    "number": "Number value",
    "displayName": "Display Name value",
    "type": "Type value",
    "address": {
      "@odata.type": "microsoft.graph.postalAddressType",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryLetterCode": "Country Letter Code value",
      "postalCode": "Postal Code value"
    },
    "phoneNumber": "Phone Number value",
    "email": "Email value",
    "website": "Website value",
    "taxLiable": true,
    "taxAreaId": "fec5ed79-ed79-fec5-79ed-c5fe79edc5fe",
    "taxAreaDisplayName": "Tax Area Display Name value",
    "taxRegistrationNumber": "Tax Registration Number value",
    "currencyId": "3fda09ad-09ad-3fda-ad09-da3fad09da3f",
    "currencyCode": "Currency Code value",
    "paymentTermsId": "699a59fb-59fb-699a-fb59-9a69fb599a69",
    "shipmentMethodId": "b9539e5d-9e5d-b953-5d9e-53b95d9e53b9",
    "paymentMethodId": "9fe5b104-b104-9fe5-04b1-e59f04b1e59f",
    "blocked": "Blocked value",
    "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00"
  }
}
```

