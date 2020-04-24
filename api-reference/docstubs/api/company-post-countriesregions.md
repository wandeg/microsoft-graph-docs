---
title: "Create countriesRegions"
description: "Create a new countriesRegions object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create countriesRegions

Namespace: microsoft.graph

Create a new countriesRegions object.

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
POST /financials/companies/{companyId}/countriesRegions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [countryRegion](../resources/countryregion.md) object.

The following table shows the properties that are required when you create the [countryRegion](../resources/countryregion.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|code|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|addressFormat|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [countryRegion](../resources/countryregion.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_countryregion_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/countriesRegions
Content-Type: application/json
Content-length: 164

{
  "@odata.type": "#microsoft.graph.countryRegion",
  "code": "Code value",
  "displayName": "Display Name value",
  "addressFormat": "Address Format value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.countryregion"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.countryRegion",
  "id": "c45db5f8-b5f8-c45d-f8b5-5dc4f8b55dc4",
  "code": "Code value",
  "displayName": "Display Name value",
  "addressFormat": "Address Format value",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
}
```

