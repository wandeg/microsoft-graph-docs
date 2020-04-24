---
title: "List customer"
description: "Get the customers from the customer navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List customer

Namespace: microsoft.graph

Get the customers from the customer navigation property.

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
GET /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/customer
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
If successful, this method returns a `200 OK` response code and a collection of [customer](../resources/customer.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_customer"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/customer
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.customer)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.customer",
      "id": "71af09c2-09c2-71af-c209-af71c209af71",
      "number": "Number value",
      "displayName": "Display Name value",
      "type": "Type value",
      "address": {
        "@odata.type": "microsoft.graph.postalAddressType",
        "street": "Street value",
        "city": "City value",
        "state": "State value",
        "countryLetterCode": "Country Letter Code value",
        "postalCode": "Postal Code value"
      },
      "phoneNumber": "Phone Number value",
      "email": "Email value",
      "website": "Website value",
      "taxLiable": true,
      "taxAreaId": "79fa183e-183e-79fa-3e18-fa793e18fa79",
      "taxAreaDisplayName": "Tax Area Display Name value",
      "taxRegistrationNumber": "Tax Registration Number value",
      "currencyId": "2bb388c6-88c6-2bb3-c688-b32bc688b32b",
      "currencyCode": "Currency Code value",
      "paymentTermsId": "54e189b4-89b4-54e1-b489-e154b489e154",
      "shipmentMethodId": "f3ea0115-0115-f3ea-1501-eaf31501eaf3",
      "paymentMethodId": "52b281a7-81a7-52b2-a781-b252a781b252",
      "blocked": "Blocked value",
      "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
    }
  ]
}
```

