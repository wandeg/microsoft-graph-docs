---
title: "List salesOrders"
description: "Get the salesOrders from the salesOrders navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List salesOrders

Namespace: microsoft.graph

Get the salesOrders from the salesOrders navigation property.

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
GET /financials/companies/{companyId}/salesOrders
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

If successful, this method returns a `200 OK` response code and a collection of [salesOrder](../resources/salesorder.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_salesorder"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesOrders
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.salesorder)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.salesOrder",
      "id": "426fe1be-e1be-426f-bee1-6f42bee16f42",
      "number": "String",
      "externalDocumentNumber": "String",
      "orderDate": "Date",
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
      "pricesIncludeTax": "Boolean",
      "paymentTermsId": "Guid",
      "salesperson": "String",
      "partialShipping": "Boolean",
      "requestedDeliveryDate": "Date",
      "discountAmount": "Decimal",
      "discountAppliedBeforeTax": "Boolean",
      "totalAmountExcludingTax": "Decimal",
      "totalTaxAmount": "Decimal",
      "totalAmountIncludingTax": "Decimal",
      "fullyShipped": "Boolean",
      "status": "String",
      "lastModifiedDateTime": "String (timestamp)",
      "phoneNumber": "String",
      "email": "String"
    }
  ]
}
```

