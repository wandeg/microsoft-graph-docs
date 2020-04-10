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
<!-- {
  "blockType": "request",
  "name": "get_salesorder"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesOrders/{salesOrderId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
    "id": "e79385b7-85b7-e793-b785-93e7b78593e7",
    "number": "Number value",
    "externalDocumentNumber": "External Document Number value",
    "orderDate": "Date",
    "customerId": "3992e4c5-e4c5-3992-c5e4-9239c5e49239",
    "customerNumber": "Customer Number value",
    "customerName": "Customer Name value",
    "billToName": "Bill To Name value",
    "billToCustomerId": "9e27a69a-a69a-9e27-9aa6-279e9aa6279e",
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
    "currencyId": "83ed47d1-47d1-83ed-d147-ed83d147ed83",
    "currencyCode": "Currency Code value",
    "pricesIncludeTax": true,
    "paymentTermsId": "be513a4b-3a4b-be51-4b3a-51be4b3a51be",
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
    "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
    "phoneNumber": "Phone Number value",
    "email": "Email value"
  }
}
```

