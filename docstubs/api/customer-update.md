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
  "taxAreaId": "165b2d40-2d40-165b-402d-5b16402d5b16",
  "taxAreaDisplayName": "Tax Area Display Name value",
  "taxRegistrationNumber": "Tax Registration Number value",
  "currencyId": "70fc6cae-6cae-70fc-ae6c-fc70ae6cfc70",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "fc178a13-8a13-fc17-138a-17fc138a17fc",
  "shipmentMethodId": "d28fd6fc-d6fc-d28f-fcd6-8fd2fcd68fd2",
  "paymentMethodId": "de8ab7af-b7af-de8a-afb7-8adeafb78ade",
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
  "id": "79aca2ce-a2ce-79ac-cea2-ac79cea2ac79",
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
  "taxAreaId": "165b2d40-2d40-165b-402d-5b16402d5b16",
  "taxAreaDisplayName": "Tax Area Display Name value",
  "taxRegistrationNumber": "Tax Registration Number value",
  "currencyId": "70fc6cae-6cae-70fc-ae6c-fc70ae6cfc70",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "fc178a13-8a13-fc17-138a-17fc138a17fc",
  "shipmentMethodId": "d28fd6fc-d6fc-d28f-fcd6-8fd2fcd68fd2",
  "paymentMethodId": "de8ab7af-b7af-de8a-afb7-8adeafb78ade",
  "blocked": "Blocked value",
  "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00"
}
```

