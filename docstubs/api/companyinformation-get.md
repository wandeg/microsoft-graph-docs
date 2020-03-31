---
title: "Get companyInformation"
description: "Read properties and relationships of the companyInformation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get companyInformation

Namespace: microsoft.graph

Read properties and relationships of the [companyInformation](../resources/companyinformation.md) object.

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
GET /financials/companies/{companyId}/companyInformation/{companyInformationId}
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
If successful, this method returns a `200 OK` response code and [companyInformation](../resources/companyinformation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_companyinformation"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/companyInformation/{companyInformationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.companyInformation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 868

{
  "value": {
    "@odata.type": "#microsoft.graph.companyInformation",
    "id": "fe032ab7-2ab7-fe03-b72a-03feb72a03fe",
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
    "lastModifiedDateTime": "2017-01-01T00:02:23.471109+03:00"
  }
}
```

