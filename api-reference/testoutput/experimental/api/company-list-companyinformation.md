---
title: "List companyInformation"
description: "Get the companyInformations from the companyInformation navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List companyInformation

Get the companyInformations from the companyInformation navigation property.

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
GET /financials/companies/{companyId}/companyInformation
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [companyInformation](../resources/companyinformation.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_companyinformation"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/financials/companies/{companyId}/companyInformation
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.companyinformation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 925

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.companyInformation",
      "id": "dc9b0c07-0c07-dc9b-070c-9bdc070c9bdc",
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
      "faxNumber": "Fax Number value",
      "email": "Email value",
      "website": "Website value",
      "taxRegistrationNumber": "Tax Registration Number value",
      "currencyCode": "Currency Code value",
      "currentFiscalYearStartDate": "Date",
      "industry": "Industry value",
      "picture": "Stream",
      "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00"
    }
  ]
}
```

