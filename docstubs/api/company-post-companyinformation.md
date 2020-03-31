---
title: "Add companyInformation"
description: "Add companyInformation by posting to the companyInformation collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add companyInformation

Namespace: microsoft.graph

Add companyInformation by posting to the companyInformation collection.

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
POST /financials/companies/{companyId}/companyInformation/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_companyinformation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/companyInformation
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
  "id": "c1f53e5c-3e5c-c1f5-5c3e-f5c15c3ef5c1",
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
  "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00"
}
```

