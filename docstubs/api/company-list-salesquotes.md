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

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /financials/companies/{companyId}/salesQuotes
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [salesQuote](../resources/salesquote.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salesquote"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesQuotes
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
      "id": "6052c4f1-c4f1-6052-f1c4-5260f1c45260",
      "number": "Number value",
      "externalDocumentNumber": "External Document Number value",
      "documentDate": "Date",
      "dueDate": "Date",
      "customerId": "9d8a53f3-53f3-9d8a-f353-8a9df3538a9d",
      "customerNumber": "Customer Number value",
      "customerName": "Customer Name value",
      "billToName": "Bill To Name value",
      "billToCustomerId": "73e9a358-a358-73e9-58a3-e97358a3e973",
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
      "currencyId": "5718300d-300d-5718-0d30-18570d301857",
      "currencyCode": "Currency Code value",
      "paymentTermsId": "ee8dd96e-d96e-ee8d-6ed9-8dee6ed98dee",
      "shipmentMethodId": "bb9ed9af-d9af-bb9e-afd9-9ebbafd99ebb",
      "salesperson": "Salesperson value",
      "discountAmount": "4.2",
      "totalAmountExcludingTax": "4.2",
      "totalTaxAmount": "4.2",
      "totalAmountIncludingTax": "4.2",
      "status": "Status value",
      "sentDate": "2016-12-31T23:57:00.3852908+03:00",
      "validUntilDate": "Date",
      "acceptedDate": "Date",
      "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
      "phoneNumber": "Phone Number value",
      "email": "Email value"
    }
  ]
}
```

