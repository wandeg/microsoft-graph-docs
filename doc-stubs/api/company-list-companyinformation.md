---
title: "List companyInformation"
description: "Get the companyInformations from the companyInformation navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List companyInformation

Namespace: microsoft.graph

Get the companyInformations from the companyInformation navigation property.

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
GET /financials/companies/{companyId}/companyInformation
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [companyInformation](../resources/companyinformation.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_companyinformation"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/companyInformation
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.companyinformation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

