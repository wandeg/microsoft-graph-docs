---
title: "Update companyInformation"
description: "Update the properties of a companyInformation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update companyInformation

Namespace: microsoft.graph

Update the properties of a [companyInformation](../resources/companyinformation.md) object.

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
PATCH /financials/companies/{companyId}/companyInformation/{companyInformationId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [companyInformation](../resources/companyinformation.md) object.

The following table shows the properties that are required when you create the [companyInformation](../resources/companyinformation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|address|[postalAddressType](../resources/postaladdresstype.md)||
|phoneNumber|String||
|faxNumber|String||
|email|String||
|website|String||
|taxRegistrationNumber|String||
|currencyCode|String||
|currentFiscalYearStartDate|Date||
|industry|String||
|picture|Stream||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [companyInformation](../resources/companyinformation.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_companyinformation"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/financials/companies/{companyId}/companyInformation/{companyInformationId}
Content-type: application/json
Content-length: 695

{
  "@odata.type": "#microsoft.graph.companyInformation",
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
  "picture": "Stream"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 808

{
  "@odata.type": "#microsoft.graph.companyInformation",
  "id": "466c1b3c-1b3c-466c-3c1b-6c463c1b6c46",
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
  "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00"
}
```

