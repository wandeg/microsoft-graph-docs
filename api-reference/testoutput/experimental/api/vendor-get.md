---
title: "Get vendor"
description: "Read properties and relationships of the vendor object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get vendor

Read properties and relationships of the [vendor](../resources/vendor.md) object.

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
GET /financials/companies/{companyId}/vendors/{vendorId}
GET /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}/vendor
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [vendor](../resources/vendor.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_vendor"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/financials/companies/{companyId}/vendors/{vendorId}
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
    "id": "500c2fbb-2fbb-500c-bb2f-0c50bb2f0c50",
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
    "currencyId": "20bf8064-8064-20bf-6480-bf206480bf20",
    "currencyCode": "Currency Code value",
    "paymentTermsId": "65ea415a-415a-65ea-5a41-ea655a41ea65",
    "paymentMethodId": "899ce3e1-e3e1-899c-e1e3-9c89e1e39c89",
    "taxLiable": true,
    "blocked": "Blocked value",
    "balance": "4.2",
    "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00"
  }
}
```

