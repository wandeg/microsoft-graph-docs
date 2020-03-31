---
title: "Update customer"
description: "Update the properties of a customer object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update customer

Namespace: microsoft.graph

Update the properties of a [customer](../resources/customer.md) object.

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
PATCH /financials/companies/{companyId}/customers/{customerId}
PATCH /financials/companies/{companyId}/salesOrders/{salesOrderId}/customer
PATCH /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/customer
PATCH /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/customer
PATCH /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/customer
PATCH /financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}/customerPayments/{customerPaymentId}/customer
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [customer](../resources/customer.md) object.

The following table shows the properties that are required when you create the [customer](../resources/customer.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|number|String||
|displayName|String||
|type|String||
|address|[postalAddressType](../resources/postaladdresstype.md)||
|phoneNumber|String||
|email|String||
|website|String||
|taxLiable|Boolean||
|taxAreaId|Guid||
|taxAreaDisplayName|String||
|taxRegistrationNumber|String||
|currencyId|Guid||
|currencyCode|String||
|paymentTermsId|Guid||
|shipmentMethodId|Guid||
|paymentMethodId|Guid||
|blocked|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [customer](../resources/customer.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_customer"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/customers/{customerId}
Content-type: application/json
Content-length: 1013

{
  "@odata.type": "#microsoft.graph.customer",
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
  "taxAreaId": "bb4e0688-0688-bb4e-8806-4ebb88064ebb",
  "taxAreaDisplayName": "Tax Area Display Name value",
  "taxRegistrationNumber": "Tax Registration Number value",
  "currencyId": "2ff7fc3c-fc3c-2ff7-3cfc-f72f3cfcf72f",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "c9d77067-7067-c9d7-6770-d7c96770d7c9",
  "shipmentMethodId": "84447efc-7efc-8444-fc7e-4484fc7e4484",
  "paymentMethodId": "b99c5e6a-5e6a-b99c-6a5e-9cb96a5e9cb9",
  "blocked": "Blocked value"
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
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.customer",
  "id": "ee531e63-1e63-ee53-631e-53ee631e53ee",
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
  "taxAreaId": "bb4e0688-0688-bb4e-8806-4ebb88064ebb",
  "taxAreaDisplayName": "Tax Area Display Name value",
  "taxRegistrationNumber": "Tax Registration Number value",
  "currencyId": "2ff7fc3c-fc3c-2ff7-3cfc-f72f3cfcf72f",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "c9d77067-7067-c9d7-6770-d7c96770d7c9",
  "shipmentMethodId": "84447efc-7efc-8444-fc7e-4484fc7e4484",
  "paymentMethodId": "b99c5e6a-5e6a-b99c-6a5e-9cb96a5e9cb9",
  "blocked": "Blocked value",
  "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00"
}
```

