---
title: "Get vendor"
description: "Read properties and relationships of the vendor object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get vendor

Namespace: microsoft.graph

Read properties and relationships of the [vendor](../resources/vendor.md) object.

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
GET /financials/companies/{companyId}/vendors/{vendorId}
GET /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}/vendor
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [vendor](../resources/vendor.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_vendor"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/vendors/{vendorId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.vendor"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1012

{
  "value": {
    "@odata.type": "#microsoft.graph.vendor",
    "id": "f8cbbdbb-bdbb-f8cb-bbbd-cbf8bbbdcbf8",
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
    "currencyId": "3fda09ad-09ad-3fda-ad09-da3fad09da3f",
    "currencyCode": "Currency Code value",
    "paymentTermsId": "699a59fb-59fb-699a-fb59-9a69fb599a69",
    "paymentMethodId": "9fe5b104-b104-9fe5-04b1-e59f04b1e59f",
    "taxLiable": true,
    "blocked": "Blocked value",
    "balance": "4.2",
    "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00"
  }
}
```

