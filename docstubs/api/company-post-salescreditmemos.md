---
title: "Add salesCreditMemos"
description: "Add salesCreditMemos by posting to the salesCreditMemos collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add salesCreditMemos

Namespace: microsoft.graph

Add salesCreditMemos by posting to the salesCreditMemos collection.

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
POST /financials/companies/{companyId}/salesCreditMemos/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [salesCreditMemo](../resources/salescreditmemo.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_salescreditmemo_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/salesCreditMemos
Content-type: application/json
Content-length: 1462

{
  "@odata.type": "#microsoft.graph.salesCreditMemo",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "creditMemoDate": "Date",
  "dueDate": "Date",
  "customerId": "8f5f13a0-13a0-8f5f-a013-5f8fa0135f8f",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "e072e734-e734-e072-34e7-72e034e772e0",
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
  "currencyId": "0727dad2-dad2-0727-d2da-2707d2da2707",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "1470d31f-d31f-1470-1fd3-70141fd37014",
  "salesperson": "Salesperson value",
  "pricesIncludeTax": true,
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "invoiceId": "64d5f2e7-f2e7-64d5-e7f2-d564e7f2d564",
  "invoiceNumber": "Invoice Number value",
  "phoneNumber": "Phone Number value",
  "email": "Email value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salescreditmemo"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1575

{
  "@odata.type": "#microsoft.graph.salesCreditMemo",
  "id": "95018648-8648-9501-4886-019548860195",
  "number": "Number value",
  "externalDocumentNumber": "External Document Number value",
  "creditMemoDate": "Date",
  "dueDate": "Date",
  "customerId": "8f5f13a0-13a0-8f5f-a013-5f8fa0135f8f",
  "customerNumber": "Customer Number value",
  "customerName": "Customer Name value",
  "billToName": "Bill To Name value",
  "billToCustomerId": "e072e734-e734-e072-34e7-72e034e772e0",
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
  "currencyId": "0727dad2-dad2-0727-d2da-2707d2da2707",
  "currencyCode": "Currency Code value",
  "paymentTermsId": "1470d31f-d31f-1470-1fd3-70141fd37014",
  "salesperson": "Salesperson value",
  "pricesIncludeTax": true,
  "discountAmount": "4.2",
  "discountAppliedBeforeTax": true,
  "totalAmountExcludingTax": "4.2",
  "totalTaxAmount": "4.2",
  "totalAmountIncludingTax": "4.2",
  "status": "Status value",
  "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
  "invoiceId": "64d5f2e7-f2e7-64d5-e7f2-d564e7f2d564",
  "invoiceNumber": "Invoice Number value",
  "phoneNumber": "Phone Number value",
  "email": "Email value"
}
```

