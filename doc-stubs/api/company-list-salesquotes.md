---
title: "List salesQuotes"
description: "Get the salesQuotes from the salesQuotes navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List salesQuotes

Namespace: microsoft.graph

Get the salesQuotes from the salesQuotes navigation property.

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
GET /financials/companies/{companyId}/salesQuotes
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [salesQuote](../resources/salesquote.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_salesquote"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesQuotes
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.salesquote)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.salesQuote",
      "id": "46f9ab2a-ab2a-46f9-2aab-f9462aabf946",
      "number": "String",
      "externalDocumentNumber": "String",
      "documentDate": "Date",
      "dueDate": "Date",
      "customerId": "Guid",
      "customerNumber": "String",
      "customerName": "String",
      "billToName": "String",
      "billToCustomerId": "Guid",
      "billToCustomerNumber": "String",
      "shipToName": "String",
      "shipToContact": "String",
      "sellingPostalAddress": {
        "@odata.type": "microsoft.graph.postalAddressType"
      },
      "billingPostalAddress": {
        "@odata.type": "microsoft.graph.postalAddressType"
      },
      "shippingPostalAddress": {
        "@odata.type": "microsoft.graph.postalAddressType"
      },
      "currencyId": "Guid",
      "currencyCode": "String",
      "paymentTermsId": "Guid",
      "shipmentMethodId": "Guid",
      "salesperson": "String",
      "discountAmount": "Decimal",
      "totalAmountExcludingTax": "Decimal",
      "totalTaxAmount": "Decimal",
      "totalAmountIncludingTax": "Decimal",
      "status": "String",
      "sentDate": "String (timestamp)",
      "validUntilDate": "Date",
      "acceptedDate": "Date",
      "lastModifiedDateTime": "String (timestamp)",
      "phoneNumber": "String",
      "email": "String"
    }
  ]
}
```

