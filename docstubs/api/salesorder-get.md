---
title: "Get salesOrder"
description: "Read properties and relationships of the salesOrder object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get salesOrder

Namespace: microsoft.graph

Read properties and relationships of the [salesOrder](../resources/salesorder.md) object.

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
GET /financials/companies/{companyId}/salesOrders/{salesOrderId}
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
If successful, this method returns a `200 OK` response code and [salesOrder](../resources/salesorder.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salesorder"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesOrders/{salesOrderId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesOrder"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1815

{
  "value": {
    "@odata.type": "#microsoft.graph.salesOrder",
    "id": "ee3a00ef-00ef-ee3a-ef00-3aeeef003aee",
    "number": "Number value",
    "externalDocumentNumber": "External Document Number value",
    "orderDate": "Date",
    "customerId": "8f5f13a0-13a0-8f5f-a013-5f8fa0135f8f",
    "customerNumber": "Customer Number value",
    "customerName": "Customer Name value",
    "billToName": "Bill To Name value",
    "billToCustomerId": "e072e734-e734-e072-34e7-72e034e772e0",
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
    "currencyId": "0727dad2-dad2-0727-d2da-2707d2da2707",
    "currencyCode": "Currency Code value",
    "pricesIncludeTax": true,
    "paymentTermsId": "1470d31f-d31f-1470-1fd3-70141fd37014",
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
    "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
    "phoneNumber": "Phone Number value",
    "email": "Email value"
  }
}
```

