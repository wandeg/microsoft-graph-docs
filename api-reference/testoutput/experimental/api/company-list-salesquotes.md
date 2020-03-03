---
title: "List salesQuotes"
description: "Get the salesQuotes from the salesQuotes navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List salesQuotes

Namespace: microsoft.graph

Get the salesQuotes from the salesQuotes navigation property.

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
GET /financials/companies/{companyId}/salesQuotes
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [salesQuote](../resources/salesquote.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salesquote"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/salesQuotes
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.salesquote)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1958

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.salesQuote",
      "id": "8ccb3257-3257-8ccb-5732-cb8c5732cb8c",
      "number": "Number value",
      "externalDocumentNumber": "External Document Number value",
      "documentDate": "Date",
      "dueDate": "Date",
      "customerId": "a61f8986-8986-a61f-8689-1fa686891fa6",
      "customerNumber": "Customer Number value",
      "customerName": "Customer Name value",
      "billToName": "Bill To Name value",
      "billToCustomerId": "7a1538dc-38dc-7a15-dc38-157adc38157a",
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
      "currencyId": "5323df69-df69-5323-69df-235369df2353",
      "currencyCode": "Currency Code value",
      "paymentTermsId": "292944c5-44c5-2929-c544-2929c5442929",
      "shipmentMethodId": "29227862-7862-2922-6278-222962782229",
      "salesperson": "Salesperson value",
      "discountAmount": "4.2",
      "totalAmountExcludingTax": "4.2",
      "totalTaxAmount": "4.2",
      "totalAmountIncludingTax": "4.2",
      "status": "Status value",
      "sentDate": "2016-12-31T23:56:36.5755901+03:00",
      "validUntilDate": "Date",
      "acceptedDate": "Date",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "phoneNumber": "Phone Number value",
      "email": "Email value"
    }
  ]
}
```

