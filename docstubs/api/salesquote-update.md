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
  "customerId": "9d8a53f3-53f3-9d8a-f353-8a9df3538a9d",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "73e9a358-a358-73e9-58a3-e97358a3e973",
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
  "currencyId": "5718300d-300d-5718-0d30-18570d301857",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "ee8dd96e-d96e-ee8d-6ed9-8dee6ed98dee",
  "shipmentMethodId": "bb9ed9af-d9af-bb9e-afd9-9ebbafd99ebb",
  "salesperson": "Salesperson value",
  "discountAmount": "4.2",
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "sentDate": "2016-12-31T23:57:00.3852908+03:00",
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
  "id": "6052c4f1-c4f1-6052-f1c4-5260f1c45260",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "documentDate": "Date",
  "dueDate": "Date",
  "customerId": "9d8a53f3-53f3-9d8a-f353-8a9df3538a9d",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "73e9a358-a358-73e9-58a3-e97358a3e973",
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
  "currencyId": "5718300d-300d-5718-0d30-18570d301857",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "ee8dd96e-d96e-ee8d-6ed9-8dee6ed98dee",
  "shipmentMethodId": "bb9ed9af-d9af-bb9e-afd9-9ebbafd99ebb",
  "salesperson": "Salesperson value",
  "discountAmount": "4.2",
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "sentDate": "2016-12-31T23:57:00.3852908+03:00",
  "validUntilDate": "Date",
  "acceptedDate": "Date",
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
  "phoneNumber": "Phone Number value",
  "email": "Email value"
}
```

