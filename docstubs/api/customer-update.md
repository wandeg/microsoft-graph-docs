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
  "taxAreaId": "6fc03a04-3a04-6fc0-043a-c06f043ac06f",
  "taxAreaDisplayName": "Tax Area Display Name value",
  "taxRegistrationNumber": "Tax Registration Number value",
  "currencyId": "83ed47d1-47d1-83ed-d147-ed83d147ed83",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "be513a4b-3a4b-be51-4b3a-51be4b3a51be",
  "shipmentMethodId": "14ada72c-a72c-14ad-2ca7-ad142ca7ad14",
  "paymentMethodId": "707810ae-10ae-7078-ae10-7870ae107870",
  "blocked": "Blocked value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
  "id": "2e9f923f-923f-2e9f-3f92-9f2e3f929f2e",
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
  "taxAreaId": "6fc03a04-3a04-6fc0-043a-c06f043ac06f",
  "taxAreaDisplayName": "Tax Area Display Name value",
  "taxRegistrationNumber": "Tax Registration Number value",
  "currencyId": "83ed47d1-47d1-83ed-d147-ed83d147ed83",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "be513a4b-3a4b-be51-4b3a-51be4b3a51be",
  "shipmentMethodId": "14ada72c-a72c-14ad-2ca7-ad142ca7ad14",
  "paymentMethodId": "707810ae-10ae-7078-ae10-7870ae107870",
  "blocked": "Blocked value",
  "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00"
}
```

