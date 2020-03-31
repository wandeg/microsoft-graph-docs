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
      "id": "9e19ce0f-ce0f-9e19-0fce-199e0fce199e",
      "number": "Number value",
      "externalDocumentNumber": "External Document Number value",
      "documentDate": "Date",
      "dueDate": "Date",
      "customerId": "820c4754-4754-820c-5447-0c8254470c82",
      "customerNumber": "Customer Number value",
      "customerName": "Customer Name value",
      "billToName": "Bill To Name value",
      "billToCustomerId": "ac36b065-b065-ac36-65b0-36ac65b036ac",
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
      "currencyId": "cf2f699a-699a-cf2f-9a69-2fcf9a692fcf",
      "currencyCode": "Currency Code value",
      "paymentTermsId": "8b180972-0972-8b18-7209-188b7209188b",
      "shipmentMethodId": "97e76ee2-6ee2-97e7-e26e-e797e26ee797",
      "salesperson": "Salesperson value",
      "discountAmount": "4.2",
      "totalAmountExcludingTax": "4.2",
      "totalTaxAmount": "4.2",
      "totalAmountIncludingTax": "4.2",
      "status": "Status value",
      "sentDate": "2016-12-31T23:59:03.5037205+03:00",
      "validUntilDate": "Date",
      "acceptedDate": "Date",
      "lastModifiedDateTime": "2017-01-01T00:01:52.9217945+03:00",
      "phoneNumber": "Phone Number value",
      "email": "Email value"
    }
  ]
}
```

