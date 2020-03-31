---
title: "Update salesQuote"
description: "Update the properties of a salesQuote object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update salesQuote

Namespace: microsoft.graph

Update the properties of a [salesQuote](../resources/salesquote.md) object.

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
PATCH /financials/companies/{companyId}/salesQuotes/{salesQuoteId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [salesQuote](../resources/salesquote.md) object.

The following table shows the properties that are required when you create the [salesQuote](../resources/salesquote.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|number|String||
|externalDocumentNumber|String||
|documentDate|Date||
|dueDate|Date||
|customerId|Guid||
|customerNumber|String||
|customerName|String||
|billToName|String||
|billToCustomerId|Guid||
|billToCustomerNumber|String||
|shipToName|String||
|shipToContact|String||
|sellingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)||
|billingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)||
|shippingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)||
|currencyId|Guid||
|currencyCode|String||
|paymentTermsId|Guid||
|shipmentMethodId|Guid||
|salesperson|String||
|discountAmount|Decimal||
|totalAmountExcludingTax|Decimal||
|totalTaxAmount|Decimal||
|totalAmountIncludingTax|Decimal||
|status|String||
|sentDate|DateTimeOffset||
|validUntilDate|Date||
|acceptedDate|Date||
|lastModifiedDateTime|DateTimeOffset||
|phoneNumber|String||
|email|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [salesQuote](../resources/salesquote.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_salesquote"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/salesQuotes/{salesQuoteId}
Content-type: application/json
Content-length: 1636

{
  "@odata.type": "#microsoft.graph.salesQuote",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "documentDate": "Date",
  "dueDate": "Date",
  "customerId": "b5483775-3775-b548-7537-48b5753748b5",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "cae7ad11-ad11-cae7-11ad-e7ca11ade7ca",
  "billToCustomerNumber": "Bill To Customer Number value",
  "shipToName": "Ship To Name value",
  "shipToContact": "Ship To Contact value",
  "sellingPostalAddress": {
    "@odata.type": "microsoft.graph.postalAddressType",
    "street": "Street value",
    "city": "City value",
    "state": "State value",
    "countryLetterCode": "Country Letter Code value",
    "postalCode": "Postal Code value"
  },
  "billingPostalAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "shippingPostalAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "currencyId": "2ff7fc3c-fc3c-2ff7-3cfc-f72f3cfcf72f",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "c9d77067-7067-c9d7-6770-d7c96770d7c9",
  "shipmentMethodId": "84447efc-7efc-8444-fc7e-4484fc7e4484",
  "salesperson": "Salesperson value",
  "discountAmount": "4.2",
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "sentDate": "2016-12-31T23:57:15.9789249+03:00",
  "validUntilDate": "Date",
  "acceptedDate": "Date",
  "phoneNumber": "Phone Number value",
  "email": "Email value"
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
Content-Length: 1749

{
  "@odata.type": "#microsoft.graph.salesQuote",
  "id": "c9014af5-4af5-c901-f54a-01c9f54a01c9",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "documentDate": "Date",
  "dueDate": "Date",
  "customerId": "b5483775-3775-b548-7537-48b5753748b5",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "cae7ad11-ad11-cae7-11ad-e7ca11ade7ca",
  "billToCustomerNumber": "Bill To Customer Number value",
  "shipToName": "Ship To Name value",
  "shipToContact": "Ship To Contact value",
  "sellingPostalAddress": {
    "@odata.type": "microsoft.graph.postalAddressType",
    "street": "Street value",
    "city": "City value",
    "state": "State value",
    "countryLetterCode": "Country Letter Code value",
    "postalCode": "Postal Code value"
  },
  "billingPostalAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "shippingPostalAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "currencyId": "2ff7fc3c-fc3c-2ff7-3cfc-f72f3cfcf72f",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "c9d77067-7067-c9d7-6770-d7c96770d7c9",
  "shipmentMethodId": "84447efc-7efc-8444-fc7e-4484fc7e4484",
  "salesperson": "Salesperson value",
  "discountAmount": "4.2",
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "sentDate": "2016-12-31T23:57:15.9789249+03:00",
  "validUntilDate": "Date",
  "acceptedDate": "Date",
  "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00",
  "phoneNumber": "Phone Number value",
  "email": "Email value"
}
```

