---
title: "Create companyInformation"
description: "Create a new companyInformation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create companyInformation

Namespace: microsoft.graph

Create a new companyInformation object.

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
POST /financials/companies/{companyId}/companyInformation
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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

If successful, this method returns a `201 Created` response code and a [companyInformation](../resources/companyinformation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_companyinformation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/companyInformation
Content-Type: application/json
Content-length: 423

{
  "@odata.type": "#microsoft.graph.companyInformation",
  "displayName": "String",
  "address": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "phoneNumber": "String",
  "faxNumber": "String",
  "email": "String",
  "website": "String",
  "taxRegistrationNumber": "String",
  "currencyCode": "String",
  "currentFiscalYearStartDate": "Date",
  "industry": "String",
  "picture": "Stream"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.companyinformation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.companyInformation",
  "id": "de560b7c-0b7c-de56-7c0b-56de7c0b56de",
  "displayName": "String",
  "address": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "phoneNumber": "String",
  "faxNumber": "String",
  "email": "String",
  "website": "String",
  "taxRegistrationNumber": "String",
  "currencyCode": "String",
  "currentFiscalYearStartDate": "Date",
  "industry": "String",
  "picture": "Stream",
  "lastModifiedDateTime": "String (timestamp)"
}
```

