---
title: "List salesOrders"
description: "Get the salesOrders from the salesOrders navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List salesOrders

Namespace: microsoft.graph

Get the salesOrders from the salesOrders navigation property.

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
GET /financials/companies/{companyId}/salesOrders
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
If successful, this method returns a `200 OK` response code and a collection of [salesOrder](../resources/salesorder.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salesorder"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesOrders
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.salesorder)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1916

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.salesOrder",
      "id": "03214e40-4e40-0321-404e-2103404e2103",
      "number": "Number value",
      "externalDocumentNumber": "External Document Number value",
      "orderDate": "Date",
      "customerId": "8abcd51d-d51d-8abc-1dd5-bc8a1dd5bc8a",
      "customerNumber": "Customer Number value",
      "customerName": "Customer Name value",
      "billToName": "Bill To Name value",
      "billToCustomerId": "fee1cc02-cc02-fee1-02cc-e1fe02cce1fe",
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
      "currencyId": "d358c210-c210-d358-10c2-58d310c258d3",
      "currencyCode": "Currency Code value",
      "pricesIncludeTax": true,
      "paymentTermsId": "2b1121b8-21b8-2b11-b821-112bb821112b",
      "salesperson": "Salesperson value",
      "partialShipping": true,
      "requestedDeliveryDate": "Date",
      "discountAmount": "4.2",
      "discountAppliedBeforeTax": true,
      "totalAmountExcludingTax": "4.2",
      "totalTaxAmount": "4.2",
      "totalAmountIncludingTax": "4.2",
      "fullyShipped": true,
      "status": "Status value",
      "lastModifiedDateTime": "2017-01-01T00:02:23.471109+03:00",
      "phoneNumber": "Phone Number value",
      "email": "Email value"
    }
  ]
}
```

