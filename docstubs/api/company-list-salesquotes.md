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
      "id": "281abc47-bc47-281a-47bc-1a2847bc1a28",
      "number": "Number value",
      "externalDocumentNumber": "External Document Number value",
      "documentDate": "Date",
      "dueDate": "Date",
      "customerId": "b905c28f-c28f-b905-8fc2-05b98fc205b9",
      "customerNumber": "Customer Number value",
      "customerName": "Customer Name value",
      "billToName": "Bill To Name value",
      "billToCustomerId": "0731f88f-f88f-0731-8ff8-31078ff83107",
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
      "currencyId": "6e55287b-287b-6e55-7b28-556e7b28556e",
      "currencyCode": "Currency Code value",
      "paymentTermsId": "c1ae039b-039b-c1ae-9b03-aec19b03aec1",
      "shipmentMethodId": "8553941a-941a-8553-1a94-53851a945385",
      "salesperson": "Salesperson value",
      "discountAmount": "4.2",
      "totalAmountExcludingTax": "4.2",
      "totalTaxAmount": "4.2",
      "totalAmountIncludingTax": "4.2",
      "status": "Status value",
      "sentDate": "2017-01-01T00:01:03.4962078+00:00",
      "validUntilDate": "Date",
      "acceptedDate": "Date",
      "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
      "phoneNumber": "Phone Number value",
      "email": "Email value"
    }
  ]
}
```

