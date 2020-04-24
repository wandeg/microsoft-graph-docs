---
title: "Update dimensionValue"
description: "Update the properties of a dimensionValue object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update dimensionValue

Namespace: microsoft.graph

Update the properties of a [dimensionValue](../resources/dimensionvalue.md) object.

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
PATCH /financials/companies/{companyId}/dimensionValues/{dimensionValueId}
PATCH /financials/companies/{companyId}/dimensions/{dimensionId}/dimensionValues/{dimensionValueId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [dimensionValue](../resources/dimensionvalue.md) object.

The following table shows the properties that are required when you create the [dimensionValue](../resources/dimensionvalue.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|code|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [dimensionValue](../resources/dimensionvalue.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_dimensionvalue"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/dimensionValues/{dimensionValueId}
Content-Type: application/json
Content-length: 121

{
  "@odata.type": "#microsoft.graph.dimensionValue",
  "code": "Code value",
  "displayName": "Display Name value"
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
  "@odata.type": "#microsoft.graph.dimensionValue",
  "id": "127d1662-1662-127d-6216-7d1262167d12",
  "code": "Code value",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
}
```

