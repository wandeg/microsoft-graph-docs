---
title: "Update salesCreditMemo"
description: "Update the properties of a salesCreditMemo object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update salesCreditMemo

Namespace: microsoft.graph

Update the properties of a [salesCreditMemo](../resources/salescreditmemo.md) object.

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
PATCH /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [salesCreditMemo](../resources/salescreditmemo.md) object.

The following table shows the properties that are required when you create the [salesCreditMemo](../resources/salescreditmemo.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|number|String||
|externalDocumentNumber|String||
|creditMemoDate|Date||
|dueDate|Date||
|customerId|Guid||
|customerNumber|String||
|customerName|String||
|billToName|String||
|billToCustomerId|Guid||
|billToCustomerNumber|String||
|sellingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)||
|billingPostalAddress|[postalAddressType](../resources/postaladdresstype.md)||
|currencyId|Guid||
|currencyCode|String||
|paymentTermsId|Guid||
|salesperson|String||
|pricesIncludeTax|Boolean||
|discountAmount|Decimal||
|discountAppliedBeforeTax|Boolean||
|totalAmountExcludingTax|Decimal||
|totalTaxAmount|Decimal||
|totalAmountIncludingTax|Decimal||
|status|String||
|lastModifiedDateTime|DateTimeOffset||
|invoiceId|Guid||
|invoiceNumber|String||
|phoneNumber|String||
|email|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [salesCreditMemo](../resources/salescreditmemo.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_salescreditmemo"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}
Content-type: application/json
Content-length: 1462

{
  "@odata.type": "#microsoft.graph.salesCreditMemo",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "creditMemoDate": "Date",
  "dueDate": "Date",
  "customerId": "b905c28f-c28f-b905-8fc2-05b98fc205b9",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "0731f88f-f88f-0731-8ff8-31078ff83107",
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
  "currencyId": "6e55287b-287b-6e55-7b28-556e7b28556e",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "c1ae039b-039b-c1ae-9b03-aec19b03aec1",
  "salesperson": "Salesperson value",
  "pricesIncludeTax": true,
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "invoiceId": "4a601be1-1be1-4a60-e11b-604ae11b604a",
  "invoiceNumber": "Invoice Number value",
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
Content-Length: 1575

{
  "@odata.type": "#microsoft.graph.salesCreditMemo",
  "id": "26324e23-4e23-2632-234e-3226234e3226",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "creditMemoDate": "Date",
  "dueDate": "Date",
  "customerId": "b905c28f-c28f-b905-8fc2-05b98fc205b9",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "0731f88f-f88f-0731-8ff8-31078ff83107",
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
  "currencyId": "6e55287b-287b-6e55-7b28-556e7b28556e",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "c1ae039b-039b-c1ae-9b03-aec19b03aec1",
  "salesperson": "Salesperson value",
  "pricesIncludeTax": true,
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
  "invoiceId": "4a601be1-1be1-4a60-e11b-604ae11b604a",
  "invoiceNumber": "Invoice Number value",
  "phoneNumber": "Phone Number value",
  "email": "Email value"
}
```

