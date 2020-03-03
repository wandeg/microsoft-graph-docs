---
title: "List customers"
description: "List properties and relationships of the customer objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List customers

Namespace: microsoft.graph

List properties and relationships of the [customer](../resources/customer.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /financials/companies/{companyId}/customers
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [customer](../resources/customer.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_customer"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/customers
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
      "id": "52a499d6-99d6-52a4-d699-a452d699a452",
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
      "taxAreaId": "592ce91b-e91b-592c-1be9-2c591be92c59",
      "taxAreaDisplayName": "Tax Area Display Name value",
      "taxRegistrationNumber": "Tax Registration Number value",
      "currencyId": "5323df69-df69-5323-69df-235369df2353",
      "currencyCode": "Currency Code value",
      "paymentTermsId": "292944c5-44c5-2929-c544-2929c5442929",
      "shipmentMethodId": "29227862-7862-2922-6278-222962782229",
      "paymentMethodId": "19caf68e-f68e-19ca-8ef6-ca198ef6ca19",
      "blocked": "Blocked value",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00"
    }
  ]
}
```

