---
title: "Create salesCreditMemos"
description: "Create a new salesCreditMemos object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create salesCreditMemos

Namespace: microsoft.graph

Create a new salesCreditMemos object.

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
POST /financials/companies/{companyId}/salesCreditMemos
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [salesCreditMemo](../resources/salescreditmemo.md) object.

The following table shows the properties that are required when you create the [salesCreditMemo](../resources/salescreditmemo.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|number|String|**TODO: Add Description**|
|externalDocumentNumber|String|**TODO: Add Description**|
|creditMemoDate|Date|**TODO: Add Description**|
|dueDate|Date|**TODO: Add Description**|
|customerId|Guid|**TODO: Add Description**|
|customerNumber|String|**TODO: Add Description**|
|customerName|String|**TODO: Add Description**|
|billToName|String|**TODO: Add Description**|
|billToCustomerId|Guid|**TODO: Add Description**|
|billToCustomerNumber|String|**TODO: Add Description**|
|sellingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|billingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|currencyId|Guid|**TODO: Add Description**|
|currencyCode|String|**TODO: Add Description**|
|paymentTermsId|Guid|**TODO: Add Description**|
|salesperson|String|**TODO: Add Description**|
|pricesIncludeTax|Boolean|**TODO: Add Description**|
|discountAmount|Decimal|**TODO: Add Description**|
|discountAppliedBeforeTax|Boolean|**TODO: Add Description**|
|totalAmountExcludingTax|Decimal|**TODO: Add Description**|
|totalTaxAmount|Decimal|**TODO: Add Description**|
|totalAmountIncludingTax|Decimal|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|invoiceId|Guid|**TODO: Add Description**|
|invoiceNumber|String|**TODO: Add Description**|
|phoneNumber|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [salesCreditMemo](../resources/salescreditmemo.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_salescreditmemo_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/salesCreditMemos
Content-Type: application/json
Content-length: 1462

{
  "@odata.type": "#microsoft.graph.salesCreditMemo",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "creditMemoDate": "Date",
  "dueDate": "Date",
  "customerId": "c235ff35-ff35-c235-35ff-35c235ff35c2",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "b9ac807c-807c-b9ac-7c80-acb97c80acb9",
  "billToCustomerNumber": "Bill To Customer Number value",
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
  "currencyId": "2bb388c6-88c6-2bb3-c688-b32bc688b32b",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "54e189b4-89b4-54e1-b489-e154b489e154",
  "salesperson": "Salesperson value",
  "pricesIncludeTax": true,
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "invoiceId": "35e90e24-0e24-35e9-240e-e935240ee935",
  "invoiceNumber": "Invoice Number value",
  "phoneNumber": "Phone Number value",
  "email": "Email value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salescreditmemo"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.salesCreditMemo",
  "id": "4feaaff7-aff7-4fea-f7af-ea4ff7afea4f",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "creditMemoDate": "Date",
  "dueDate": "Date",
  "customerId": "c235ff35-ff35-c235-35ff-35c235ff35c2",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "b9ac807c-807c-b9ac-7c80-acb97c80acb9",
  "billToCustomerNumber": "Bill To Customer Number value",
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
  "currencyId": "2bb388c6-88c6-2bb3-c688-b32bc688b32b",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "54e189b4-89b4-54e1-b489-e154b489e154",
  "salesperson": "Salesperson value",
  "pricesIncludeTax": true,
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "invoiceId": "35e90e24-0e24-35e9-240e-e935240ee935",
  "invoiceNumber": "Invoice Number value",
  "phoneNumber": "Phone Number value",
  "email": "Email value"
}
```

