---
title: "Get countryRegion"
description: "Read the properties and relationships of a countryRegion object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get countryRegion

Namespace: microsoft.graph

Read the properties and relationships of a [countryRegion](../resources/countryregion.md) object.

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
GET /financials/companies/{companyId}/countriesRegions/{countryRegionId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [countryRegion](../resources/countryregion.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_countryregion"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/countriesRegions/{countryRegionId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.countryRegion"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.countryRegion",
    "id": "c45db5f8-b5f8-c45d-f8b5-5dc4f8b55dc4",
    "code": "Code value",
    "displayName": "Display Name value",
    "addressFormat": "Address Format value",
    "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
  }
}
```

