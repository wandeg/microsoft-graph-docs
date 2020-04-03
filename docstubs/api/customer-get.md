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
|Name|Description|
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
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/customers/{customerId}
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
    "id": "3ea5343a-343a-3ea5-3a34-a53e3a34a53e",
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
    "taxAreaId": "d867fdc0-fdc0-d867-c0fd-67d8c0fd67d8",
    "taxAreaDisplayName": "Tax Area Display Name value",
    "taxRegistrationNumber": "Tax Registration Number value",
    "currencyId": "6e55287b-287b-6e55-7b28-556e7b28556e",
    "currencyCode": "Currency Code value",
    "paymentTermsId": "c1ae039b-039b-c1ae-9b03-aec19b03aec1",
    "shipmentMethodId": "8553941a-941a-8553-1a94-53851a945385",
    "paymentMethodId": "199aeaed-eaed-199a-edea-9a19edea9a19",
    "blocked": "Blocked value",
    "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00"
  }
}
```

