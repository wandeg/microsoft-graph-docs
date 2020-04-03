---
title: "Update salesOrder"
description: "Update the properties of a salesOrder object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update salesOrder

Namespace: microsoft.graph

Update the properties of a [salesOrder](../resources/salesorder.md) object.

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
PATCH /financials/companies/{companyId}/salesOrders/{salesOrderId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [salesOrder](../resources/salesorder.md) object.

The following table shows the properties that are required when you create the [salesOrder](../resources/salesorder.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|number|String||
|externalDocumentNumber|String||
|orderDate|Date||
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
|pricesIncludeTax|Boolean||
|paymentTermsId|Guid||
|salesperson|String||
|partialShipping|Boolean||
|requestedDeliveryDate|Date||
|discountAmount|Decimal||
|discountAppliedBeforeTax|Boolean||
|totalAmountExcludingTax|Decimal||
|totalTaxAmount|Decimal||
|totalAmountIncludingTax|Decimal||
|fullyShipped|Boolean||
|status|String||
|lastModifiedDateTime|DateTimeOffset||
|phoneNumber|String||
|email|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [salesOrder](../resources/salesorder.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_salesorder"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/salesOrders/{salesOrderId}
Content-type: application/json
Content-length: 1595

{
  "@odata.type": "#microsoft.graph.salesOrder",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "orderDate": "Date",
  "customerId": "b905c28f-c28f-b905-8fc2-05b98fc205b9",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "0731f88f-f88f-0731-8ff8-31078ff83107",
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
  "currencyId": "6e55287b-287b-6e55-7b28-556e7b28556e",
  "currencyCode": "Currency Code value",
  "pricesIncludeTax": true,
  "paymentTermsId": "c1ae039b-039b-c1ae-9b03-aec19b03aec1",
  "salesperson": "Salesperson value",
  "partialShipping": true,
  "requestedDeliveryDate": "Date",
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "fullyShipped": true,
  "status": "Status value",
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
Content-Length: 1708

{
  "@odata.type": "#microsoft.graph.salesOrder",
  "id": "5cbf69e0-69e0-5cbf-e069-bf5ce069bf5c",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "orderDate": "Date",
  "customerId": "b905c28f-c28f-b905-8fc2-05b98fc205b9",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "0731f88f-f88f-0731-8ff8-31078ff83107",
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
  "currencyId": "6e55287b-287b-6e55-7b28-556e7b28556e",
  "currencyCode": "Currency Code value",
  "pricesIncludeTax": true,
  "paymentTermsId": "c1ae039b-039b-c1ae-9b03-aec19b03aec1",
  "salesperson": "Salesperson value",
  "partialShipping": true,
  "requestedDeliveryDate": "Date",
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "fullyShipped": true,
  "status": "Status value",
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
  "phoneNumber": "Phone Number value",
  "email": "Email value"
}
```

