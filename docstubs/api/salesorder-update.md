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
  "customerId": "3992e4c5-e4c5-3992-c5e4-9239c5e49239",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "9e27a69a-a69a-9e27-9aa6-279e9aa6279e",
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
  "currencyId": "83ed47d1-47d1-83ed-d147-ed83d147ed83",
  "currencyCode": "Currency Code value",
  "pricesIncludeTax": true,
  "paymentTermsId": "be513a4b-3a4b-be51-4b3a-51be4b3a51be",
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
  "id": "e79385b7-85b7-e793-b785-93e7b78593e7",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "orderDate": "Date",
  "customerId": "3992e4c5-e4c5-3992-c5e4-9239c5e49239",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "9e27a69a-a69a-9e27-9aa6-279e9aa6279e",
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
  "currencyId": "83ed47d1-47d1-83ed-d147-ed83d147ed83",
  "currencyCode": "Currency Code value",
  "pricesIncludeTax": true,
  "paymentTermsId": "be513a4b-3a4b-be51-4b3a-51be4b3a51be",
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
  "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
  "phoneNumber": "Phone Number value",
  "email": "Email value"
}
```

