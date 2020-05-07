---
title: "Create salesOrders"
description: "Create a new salesOrders object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create salesOrders

Namespace: microsoft.graph

Create a new salesOrders object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /financials/companies/{companyId}/salesOrders
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [salesOrder](../resources/salesorder.md) object.

The following table shows the properties that are required when you create the [salesOrder](../resources/salesorder.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|number|String|**TODO: Add Description**|
|externalDocumentNumber|String|**TODO: Add Description**|
|orderDate|Date|**TODO: Add Description**|
|customerId|Guid|**TODO: Add Description**|
|customerNumber|String|**TODO: Add Description**|
|customerName|String|**TODO: Add Description**|
|billToName|String|**TODO: Add Description**|
|billToCustomerId|Guid|**TODO: Add Description**|
|billToCustomerNumber|String|**TODO: Add Description**|
|shipToName|String|**TODO: Add Description**|
|shipToContact|String|**TODO: Add Description**|
|sellingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|billingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|shippingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|currencyId|Guid|**TODO: Add Description**|
|currencyCode|String|**TODO: Add Description**|
|pricesIncludeTax|Boolean|**TODO: Add Description**|
|paymentTermsId|Guid|**TODO: Add Description**|
|salesperson|String|**TODO: Add Description**|
|partialShipping|Boolean|**TODO: Add Description**|
|requestedDeliveryDate|Date|**TODO: Add Description**|
|discountAmount|Decimal|**TODO: Add Description**|
|discountAppliedBeforeTax|Boolean|**TODO: Add Description**|
|totalAmountExcludingTax|Decimal|**TODO: Add Description**|
|totalTaxAmount|Decimal|**TODO: Add Description**|
|totalAmountIncludingTax|Decimal|**TODO: Add Description**|
|fullyShipped|Boolean|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|phoneNumber|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [salesOrder](../resources/salesorder.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_salesorder_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/salesOrders
Content-Type: application/json
Content-length: 1154

{
  "@odata.type": "#microsoft.graph.salesOrder",
  "number": "String",
  "externalDocumentNumber": "String",
  "orderDate": "Date",
  "customerId": "Guid",
  "customerNumber": "String",
  "customerName": "String",
  "billToName": "String",
  "billToCustomerId": "Guid",
  "billToCustomerNumber": "String",
  "shipToName": "String",
  "shipToContact": "String",
  "sellingPostalAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "billingPostalAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "shippingPostalAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "currencyId": "Guid",
  "currencyCode": "String",
  "pricesIncludeTax": "Boolean",
  "paymentTermsId": "Guid",
  "salesperson": "String",
  "partialShipping": "Boolean",
  "requestedDeliveryDate": "Date",
  "discountAmount": "Decimal",
  "discountAppliedBeforeTax": "Boolean",
  "totalAmountExcludingTax": "Decimal",
  "totalTaxAmount": "Decimal",
  "totalAmountIncludingTax": "Decimal",
  "fullyShipped": "Boolean",
  "status": "String",
  "phoneNumber": "String",
  "email": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesorder"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.salesOrder",
  "id": "426fe1be-e1be-426f-bee1-6f42bee16f42",
  "number": "String",
  "externalDocumentNumber": "String",
  "orderDate": "Date",
  "customerId": "Guid",
  "customerNumber": "String",
  "customerName": "String",
  "billToName": "String",
  "billToCustomerId": "Guid",
  "billToCustomerNumber": "String",
  "shipToName": "String",
  "shipToContact": "String",
  "sellingPostalAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "billingPostalAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "shippingPostalAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "currencyId": "Guid",
  "currencyCode": "String",
  "pricesIncludeTax": "Boolean",
  "paymentTermsId": "Guid",
  "salesperson": "String",
  "partialShipping": "Boolean",
  "requestedDeliveryDate": "Date",
  "discountAmount": "Decimal",
  "discountAppliedBeforeTax": "Boolean",
  "totalAmountExcludingTax": "Decimal",
  "totalTaxAmount": "Decimal",
  "totalAmountIncludingTax": "Decimal",
  "fullyShipped": "Boolean",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "phoneNumber": "String",
  "email": "String"
}
```

