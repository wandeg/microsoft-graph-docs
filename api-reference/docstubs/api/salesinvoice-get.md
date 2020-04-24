---
title: "Get salesInvoice"
description: "Read the properties and relationships of a salesInvoice object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get salesInvoice

Namespace: microsoft.graph

Read the properties and relationships of a [salesInvoice](../resources/salesinvoice.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [salesInvoice](../resources/salesinvoice.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_salesinvoice"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesInvoices/{salesInvoiceId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesInvoice"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.salesInvoice",
    "id": "ac24cb55-cb55-ac24-55cb-24ac55cb24ac",
    "number": "Number value",
    "externalDocumentNumber": "External Document Number value",
    "invoiceDate": "Date",
    "dueDate": "Date",
    "customerPurchaseOrderReference": "Customer Purchase Order Reference value",
    "customerId": "c235ff35-ff35-c235-35ff-35c235ff35c2",
    "customerNumber": "Customer Number value",
    "customerName": "Customer Name value",
    "billToName": "Bill To Name value",
    "billToCustomerId": "b9ac807c-807c-b9ac-7c80-acb97c80acb9",
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
    "currencyId": "2bb388c6-88c6-2bb3-c688-b32bc688b32b",
    "currencyCode": "Currency Code value",
    "orderId": "6a4bc437-c437-6a4b-37c4-4b6a37c44b6a",
    "orderNumber": "Order Number value",
    "paymentTermsId": "54e189b4-89b4-54e1-b489-e154b489e154",
    "shipmentMethodId": "f3ea0115-0115-f3ea-1501-eaf31501eaf3",
    "salesperson": "Salesperson value",
    "pricesIncludeTax": true,
    "discountAmount": "4.2",
    "discountAppliedBeforeTax": true,
    "totalAmountExcludingTax": "4.2",
    "totalTaxAmount": "4.2",
    "totalAmountIncludingTax": "4.2",
    "status": "Status value",
    "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
    "phoneNumber": "Phone Number value",
    "email": "Email value"
  }
}
```

