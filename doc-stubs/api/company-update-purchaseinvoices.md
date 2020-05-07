---
title: "Update purchaseInvoices"
description: "Update the properties of a purchaseInvoices object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update purchaseInvoices

Namespace: microsoft.graph

Update the properties of a purchaseInvoices object.

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
PATCH /financials/companies/{companyId}/purchaseInvoices
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [purchaseInvoice](../resources/purchaseinvoice.md) object.

The following table shows the properties that are required when you create the [purchaseInvoice](../resources/purchaseinvoice.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|number|String|**TODO: Add Description**|
|invoiceDate|Date|**TODO: Add Description**|
|dueDate|Date|**TODO: Add Description**|
|vendorInvoiceNumber|String|**TODO: Add Description**|
|vendorId|Guid|**TODO: Add Description**|
|vendorNumber|String|**TODO: Add Description**|
|vendorName|String|**TODO: Add Description**|
|payToName|String|**TODO: Add Description**|
|payToContact|String|**TODO: Add Description**|
|payToVendorId|Guid|**TODO: Add Description**|
|payToVendorNumber|String|**TODO: Add Description**|
|shipToName|String|**TODO: Add Description**|
|shipToContact|String|**TODO: Add Description**|
|buyFromAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|payToAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|shipToAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|currencyId|Guid|**TODO: Add Description**|
|currencyCode|String|**TODO: Add Description**|
|pricesIncludeTax|Boolean|**TODO: Add Description**|
|discountAmount|Decimal|**TODO: Add Description**|
|discountAppliedBeforeTax|Boolean|**TODO: Add Description**|
|totalAmountExcludingTax|Decimal|**TODO: Add Description**|
|totalTaxAmount|Decimal|**TODO: Add Description**|
|totalAmountIncludingTax|Decimal|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [purchaseInvoice](../resources/purchaseinvoice.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_purchaseinvoices"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/purchaseInvoices
Content-Type: application/json
Content-length: 968

{
  "@odata.type": "#microsoft.graph.purchaseInvoice",
  "number": "String",
  "invoiceDate": "Date",
  "dueDate": "Date",
  "vendorInvoiceNumber": "String",
  "vendorId": "Guid",
  "vendorNumber": "String",
  "vendorName": "String",
  "payToName": "String",
  "payToContact": "String",
  "payToVendorId": "Guid",
  "payToVendorNumber": "String",
  "shipToName": "String",
  "shipToContact": "String",
  "buyFromAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "payToAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "shipToAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "currencyId": "Guid",
  "currencyCode": "String",
  "pricesIncludeTax": "Boolean",
  "discountAmount": "Decimal",
  "discountAppliedBeforeTax": "Boolean",
  "totalAmountExcludingTax": "Decimal",
  "totalTaxAmount": "Decimal",
  "totalAmountIncludingTax": "Decimal",
  "status": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.purchaseInvoice",
  "id": "fcefc424-c424-fcef-24c4-effc24c4effc",
  "number": "String",
  "invoiceDate": "Date",
  "dueDate": "Date",
  "vendorInvoiceNumber": "String",
  "vendorId": "Guid",
  "vendorNumber": "String",
  "vendorName": "String",
  "payToName": "String",
  "payToContact": "String",
  "payToVendorId": "Guid",
  "payToVendorNumber": "String",
  "shipToName": "String",
  "shipToContact": "String",
  "buyFromAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "payToAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "shipToAddress": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "currencyId": "Guid",
  "currencyCode": "String",
  "pricesIncludeTax": "Boolean",
  "discountAmount": "Decimal",
  "discountAppliedBeforeTax": "Boolean",
  "totalAmountExcludingTax": "Decimal",
  "totalTaxAmount": "Decimal",
  "totalAmountIncludingTax": "Decimal",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

