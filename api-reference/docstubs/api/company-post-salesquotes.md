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
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
Content-length: 1636

{
  "@odata.type": "#microsoft.graph.salesQuote",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "documentDate": "Date",
  "dueDate": "Date",
  "customerId": "c235ff35-ff35-c235-35ff-35c235ff35c2",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "b9ac807c-807c-b9ac-7c80-acb97c80acb9",
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
  "currencyId": "2bb388c6-88c6-2bb3-c688-b32bc688b32b",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "54e189b4-89b4-54e1-b489-e154b489e154",
  "shipmentMethodId": "f3ea0115-0115-f3ea-1501-eaf31501eaf3",
  "salesperson": "Salesperson value",
  "discountAmount": "4.2",
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "sentDate": "2016-12-31T23:57:45.4131316+03:00",
  "validUntilDate": "Date",
  "acceptedDate": "Date",
  "phoneNumber": "Phone Number value",
  "email": "Email value"
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
  "id": "fc4064d5-64d5-fc40-d564-40fcd56440fc",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "documentDate": "Date",
  "dueDate": "Date",
  "customerId": "c235ff35-ff35-c235-35ff-35c235ff35c2",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "b9ac807c-807c-b9ac-7c80-acb97c80acb9",
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
  "currencyId": "2bb388c6-88c6-2bb3-c688-b32bc688b32b",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "54e189b4-89b4-54e1-b489-e154b489e154",
  "shipmentMethodId": "f3ea0115-0115-f3ea-1501-eaf31501eaf3",
  "salesperson": "Salesperson value",
  "discountAmount": "4.2",
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "sentDate": "2016-12-31T23:57:45.4131316+03:00",
  "validUntilDate": "Date",
  "acceptedDate": "Date",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "phoneNumber": "Phone Number value",
  "email": "Email value"
}
```

