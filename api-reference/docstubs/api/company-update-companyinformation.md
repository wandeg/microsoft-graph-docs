---
title: "Update companyInformation"
description: "Update the properties of a companyInformation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update companyInformation

Namespace: microsoft.graph

Update the properties of a companyInformation object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /financials/companies/{companyId}/companyInformation
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [companyInformation](../resources/companyinformation.md) object.

The following table shows the properties that are required when you create the [companyInformation](../resources/companyinformation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|address|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|phoneNumber|String|**TODO: Add Description**|
|faxNumber|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|website|String|**TODO: Add Description**|
|taxRegistrationNumber|String|**TODO: Add Description**|
|currencyCode|String|**TODO: Add Description**|
|currentFiscalYearStartDate|Date|**TODO: Add Description**|
|industry|String|**TODO: Add Description**|
|picture|Stream|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [companyInformation](../resources/companyinformation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_companyinformation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/companyInformation
Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.companyInformation",
  "id": "1d225e90-5e90-1d22-905e-221d905e221d",
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
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
}
```

