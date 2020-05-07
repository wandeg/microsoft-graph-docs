---
title: "Create salesInvoices"
description: "Create a new salesInvoices object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create salesInvoices

Namespace: microsoft.graph

Create a new salesInvoices object.

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
POST /financials/companies/{companyId}/salesInvoices
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [salesInvoice](../resources/salesinvoice.md) object.

The following table shows the properties that are required when you create the [salesInvoice](../resources/salesinvoice.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|number|String|**TODO: Add Description**|
|externalDocumentNumber|String|**TODO: Add Description**|
|invoiceDate|Date|**TODO: Add Description**|
|dueDate|Date|**TODO: Add Description**|
|customerPurchaseOrderReference|String|**TODO: Add Description**|
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
|orderId|Guid|**TODO: Add Description**|
|orderNumber|String|**TODO: Add Description**|
|paymentTermsId|Guid|**TODO: Add Description**|
|shipmentMethodId|Guid|**TODO: Add Description**|
|salesperson|String|**TODO: Add Description**|
|pricesIncludeTax|Boolean|**TODO: Add Description**|
|discountAmount|Decimal|**TODO: Add Description**|
|discountAppliedBeforeTax|Boolean|**TODO: Add Description**|
|totalAmountExcludingTax|Decimal|**TODO: Add Description**|
|totalTaxAmount|Decimal|**TODO: Add Description**|
|totalAmountIncludingTax|Decimal|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|phoneNumber|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [salesInvoice](../resources/salesinvoice.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_salesinvoice_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/salesInvoices
Content-Type: application/json
Content-length: 1209

{
  "@odata.type": "#microsoft.graph.salesInvoice",
  "number": "String",
  "externalDocumentNumber": "String",
  "invoiceDate": "Date",
  "dueDate": "Date",
  "customerPurchaseOrderReference": "String",
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
  "orderId": "Guid",
  "orderNumber": "String",
  "paymentTermsId": "Guid",
  "shipmentMethodId": "Guid",
  "salesperson": "String",
  "pricesIncludeTax": "Boolean",
  "discountAmount": "Decimal",
  "discountAppliedBeforeTax": "Boolean",
  "totalAmountExcludingTax": "Decimal",
  "totalTaxAmount": "Decimal",
  "totalAmountIncludingTax": "Decimal",
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
  "@odata.type": "microsoft.graph.salesinvoice"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.salesInvoice",
  "id": "61e433c6-33c6-61e4-c633-e461c633e461",
  "number": "String",
  "externalDocumentNumber": "String",
  "invoiceDate": "Date",
  "dueDate": "Date",
  "customerPurchaseOrderReference": "String",
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
  "orderId": "Guid",
  "orderNumber": "String",
  "paymentTermsId": "Guid",
  "shipmentMethodId": "Guid",
  "salesperson": "String",
  "pricesIncludeTax": "Boolean",
  "discountAmount": "Decimal",
  "discountAppliedBeforeTax": "Boolean",
  "totalAmountExcludingTax": "Decimal",
  "totalTaxAmount": "Decimal",
  "totalAmountIncludingTax": "Decimal",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "phoneNumber": "String",
  "email": "String"
}
```

