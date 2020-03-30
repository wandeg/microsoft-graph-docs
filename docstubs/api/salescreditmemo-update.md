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
  "customerId": "9d8a53f3-53f3-9d8a-f353-8a9df3538a9d",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "73e9a358-a358-73e9-58a3-e97358a3e973",
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
  "currencyId": "5718300d-300d-5718-0d30-18570d301857",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "ee8dd96e-d96e-ee8d-6ed9-8dee6ed98dee",
  "salesperson": "Salesperson value",
  "pricesIncludeTax": true,
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "invoiceId": "df924d61-4d61-df92-614d-92df614d92df",
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
  "id": "7ac55bf7-5bf7-7ac5-f75b-c57af75bc57a",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "creditMemoDate": "Date",
  "dueDate": "Date",
  "customerId": "9d8a53f3-53f3-9d8a-f353-8a9df3538a9d",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "73e9a358-a358-73e9-58a3-e97358a3e973",
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
  "currencyId": "5718300d-300d-5718-0d30-18570d301857",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "ee8dd96e-d96e-ee8d-6ed9-8dee6ed98dee",
  "salesperson": "Salesperson value",
  "pricesIncludeTax": true,
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
  "invoiceId": "df924d61-4d61-df92-614d-92df614d92df",
  "invoiceNumber": "Invoice Number value",
  "phoneNumber": "Phone Number value",
  "email": "Email value"
}
```

