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
      "id": "c527f3a5-f3a5-c527-a5f3-27c5a5f327c5",
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
      "taxAreaId": "cb5428c8-28c8-cb54-c828-54cbc82854cb",
      "taxAreaDisplayName": "Tax Area Display Name value",
      "taxRegistrationNumber": "Tax Registration Number value",
      "currencyId": "0727dad2-dad2-0727-d2da-2707d2da2707",
      "currencyCode": "Currency Code value",
      "paymentTermsId": "1470d31f-d31f-1470-1fd3-70141fd37014",
      "shipmentMethodId": "a8a54da3-4da3-a8a5-a34d-a5a8a34da5a8",
      "paymentMethodId": "65d93237-3237-65d9-3732-d9653732d965",
      "blocked": "Blocked value",
      "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00"
    }
  ]
}
```

