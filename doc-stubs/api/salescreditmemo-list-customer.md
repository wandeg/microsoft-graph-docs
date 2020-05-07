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
GET /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/customer
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

If successful, this method returns a `200 OK` response code and a collection of [customer](../resources/customer.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_customer"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/customer
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
      "id": "7b7faf36-af36-7b7f-36af-7f7b36af7f7b",
      "number": "String",
      "displayName": "String",
      "type": "String",
      "address": {
        "@odata.type": "microsoft.graph.postalAddressType"
      },
      "phoneNumber": "String",
      "email": "String",
      "website": "String",
      "taxLiable": "Boolean",
      "taxAreaId": "Guid",
      "taxAreaDisplayName": "String",
      "taxRegistrationNumber": "String",
      "currencyId": "Guid",
      "currencyCode": "String",
      "paymentTermsId": "Guid",
      "shipmentMethodId": "Guid",
      "paymentMethodId": "Guid",
      "blocked": "String",
      "lastModifiedDateTime": "String (timestamp)"
    }
  ]
}
```

