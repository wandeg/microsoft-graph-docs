---
title: "List customers"
description: "Get the customers from the customers navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List customers

Namespace: microsoft.graph

Get the customers from the customers navigation property.

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
GET /financials/companies/{companyId}/customers
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
If successful, this method returns a `200 OK` response code and a collection of [customer](../resources/customer.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_customer"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/customers
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.customer)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1267

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.customer",
      "id": "8c9c493c-493c-8c9c-3c49-9c8c3c499c8c",
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
      "taxAreaId": "6149d67c-d67c-6149-7cd6-49617cd64961",
      "taxAreaDisplayName": "Tax Area Display Name value",
      "taxRegistrationNumber": "Tax Registration Number value",
      "currencyId": "5718300d-300d-5718-0d30-18570d301857",
      "currencyCode": "Currency Code value",
      "paymentTermsId": "ee8dd96e-d96e-ee8d-6ed9-8dee6ed98dee",
      "shipmentMethodId": "bb9ed9af-d9af-bb9e-afd9-9ebbafd99ebb",
      "paymentMethodId": "9309ed2d-ed2d-9309-2ded-09932ded0993",
      "blocked": "Blocked value",
      "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00"
    }
  ]
}
```

