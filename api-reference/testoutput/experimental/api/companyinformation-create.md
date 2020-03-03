---
title: "Create companyInformation"
description: "Create a new companyInformation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create companyInformation

Namespace: microsoft.graph

Create a new [companyInformation](../resources/companyinformation.md) object.

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
POST /financials/companies/{companyId}/companyInformation
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
If successful, this method returns a `201 Created` response code and a [companyInformation](../resources/companyinformation.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_companyinformation_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/financials/companies/{companyId}/companyInformation
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
  "truncated": true,
  "@odata.type": "microsoft.graph.companyinformation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 808

{
  "@odata.type": "#microsoft.graph.companyInformation",
  "id": "d65a8cc1-8cc1-d65a-c18c-5ad6c18c5ad6",
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
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00"
}
```

