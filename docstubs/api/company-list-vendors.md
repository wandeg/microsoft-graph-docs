---
title: "List vendors"
description: "Get the vendors from the vendors navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List vendors

Namespace: microsoft.graph

Get the vendors from the vendors navigation property.

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
GET /financials/companies/{companyId}/vendors
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
If successful, this method returns a `200 OK` response code and a collection of [vendor](../resources/vendor.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_vendor"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/vendors
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.vendor)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1074

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.vendor",
      "id": "6c0dbb8e-bb8e-6c0d-8ebb-0d6c8ebb0d6c",
      "number": "Number value",
      "displayName": "Display Name value",
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
      "taxRegistrationNumber": "Tax Registration Number value",
      "currencyId": "2ff7fc3c-fc3c-2ff7-3cfc-f72f3cfcf72f",
      "currencyCode": "Currency Code value",
      "paymentTermsId": "c9d77067-7067-c9d7-6770-d7c96770d7c9",
      "paymentMethodId": "b99c5e6a-5e6a-b99c-6a5e-9cb96a5e9cb9",
      "taxLiable": true,
      "blocked": "Blocked value",
      "balance": "4.2",
      "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00"
    }
  ]
}
```

