---
title: "Create salesQuotes"
description: "Create a new salesQuotes object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create salesQuotes

Namespace: microsoft.graph

Create a new salesQuotes object.

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
POST /financials/companies/{companyId}/salesQuotes
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [salesQuote](../resources/salesquote.md) object.

The following table shows the properties that are required when you create the [salesQuote](../resources/salesquote.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|number|String|**TODO: Add Description**|
|externalDocumentNumber|String|**TODO: Add Description**|
|documentDate|Date|**TODO: Add Description**|
|dueDate|Date|**TODO: Add Description**|
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
|paymentTermsId|Guid|**TODO: Add Description**|
|shipmentMethodId|Guid|**TODO: Add Description**|
|salesperson|String|**TODO: Add Description**|
|discountAmount|Decimal|**TODO: Add Description**|
|totalAmountExcludingTax|Decimal|**TODO: Add Description**|
|totalTaxAmount|Decimal|**TODO: Add Description**|
|totalAmountIncludingTax|Decimal|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|sentDate|DateTimeOffset|**TODO: Add Description**|
|validUntilDate|Date|**TODO: Add Description**|
|acceptedDate|Date|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|phoneNumber|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [salesQuote](../resources/salesquote.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_salesquote_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/salesQuotes
Content-Type: application/json
Content-length: 1128

{
  "@odata.type": "#microsoft.graph.salesQuote",
  "number": "String",
  "externalDocumentNumber": "String",
  "documentDate": "Date",
  "dueDate": "Date",
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
  "paymentTermsId": "Guid",
  "shipmentMethodId": "Guid",
  "salesperson": "String",
  "discountAmount": "Decimal",
  "totalAmountExcludingTax": "Decimal",
  "totalTaxAmount": "Decimal",
  "totalAmountIncludingTax": "Decimal",
  "status": "String",
  "sentDate": "String (timestamp)",
  "validUntilDate": "Date",
  "acceptedDate": "Date",
  "phoneNumber": "String",
  "email": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesquote"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.salesQuote",
  "id": "46f9ab2a-ab2a-46f9-2aab-f9462aabf946",
  "number": "String",
  "externalDocumentNumber": "String",
  "documentDate": "Date",
  "dueDate": "Date",
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
  "paymentTermsId": "Guid",
  "shipmentMethodId": "Guid",
  "salesperson": "String",
  "discountAmount": "Decimal",
  "totalAmountExcludingTax": "Decimal",
  "totalTaxAmount": "Decimal",
  "totalAmountIncludingTax": "Decimal",
  "status": "String",
  "sentDate": "String (timestamp)",
  "validUntilDate": "Date",
  "acceptedDate": "Date",
  "lastModifiedDateTime": "String (timestamp)",
  "phoneNumber": "String",
  "email": "String"
}
```

