---
title: "Add salesOrders"
description: "Add salesOrders by posting to the salesOrders collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add salesOrders

Namespace: microsoft.graph

Add salesOrders by posting to the salesOrders collection.

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
POST /financials/companies/{companyId}/salesOrders/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [salesOrder](../resources/salesorder.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_salesorder_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/salesOrders
Content-type: application/json
Content-length: 1595

{
  "@odata.type": "#microsoft.graph.salesOrder",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "orderDate": "Date",
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
  "pricesIncludeTax": true,
  "paymentTermsId": "c9d77067-7067-c9d7-6770-d7c96770d7c9",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.salesorder"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1708

{
  "@odata.type": "#microsoft.graph.salesOrder",
  "id": "c66565c8-65c8-c665-c865-65c6c86565c6",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "orderDate": "Date",
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
  "pricesIncludeTax": true,
  "paymentTermsId": "c9d77067-7067-c9d7-6770-d7c96770d7c9",
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
  "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00",
  "phoneNumber": "Phone Number value",
  "email": "Email value"
}
```

