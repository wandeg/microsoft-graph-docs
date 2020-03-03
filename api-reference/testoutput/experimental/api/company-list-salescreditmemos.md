---
title: "List salesCreditMemos"
description: "Get the salesCreditMemos from the salesCreditMemos navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List salesCreditMemos

Get the salesCreditMemos from the salesCreditMemos navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /financials/companies/{companyId}/salesCreditMemos
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [salesCreditMemo](../resources/salescreditmemo.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salescreditmemo"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/financials/companies/{companyId}/salesCreditMemos
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.salescreditmemo)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1764

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.salesCreditMemo",
      "id": "27d1a4ee-a4ee-27d1-eea4-d127eea4d127",
      "number": "Number value",
      "externalDocumentNumber": "External Document Number value",
      "creditMemoDate": "Date",
      "dueDate": "Date",
      "customerId": "c49f9156-9156-c49f-5691-9fc456919fc4",
      "customerNumber": "Customer Number value",
      "customerName": "Customer Name value",
      "billToName": "Bill To Name value",
      "billToCustomerId": "3f40489e-489e-3f40-9e48-403f9e48403f",
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
      "currencyId": "20bf8064-8064-20bf-6480-bf206480bf20",
      "currencyCode": "Currency Code value",
      "paymentTermsId": "65ea415a-415a-65ea-5a41-ea655a41ea65",
      "salesperson": "Salesperson value",
      "pricesIncludeTax": true,
      "discountAmount": "4.2",
      "discountAppliedBeforeTax": true,
      "totalAmountExcludingTax": "4.2",
      "totalTaxAmount": "4.2",
      "totalAmountIncludingTax": "4.2",
      "status": "Status value",
      "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
      "invoiceId": "f237e20c-e20c-f237-0ce2-37f20ce237f2",
      "invoiceNumber": "Invoice Number value",
      "phoneNumber": "Phone Number value",
      "email": "Email value"
    }
  ]
}
```

