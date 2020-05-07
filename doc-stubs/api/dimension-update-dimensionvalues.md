---
title: "Update dimensionValues"
description: "Update the properties of a dimensionValues object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update dimensionValues

Namespace: microsoft.graph

Update the properties of a dimensionValues object.

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
PATCH /financials/companies/{companyId}/dimensions/{dimensionId}/dimensionValues
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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
  "name": "update_dimensionvalues"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/dimensions/{dimensionId}/dimensionValues
Content-Type: application/json
Content-length: 105

{
  "@odata.type": "#microsoft.graph.dimensionValue",
  "code": "String",
  "displayName": "String"
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
  "id": "7fa0c630-c630-7fa0-30c6-a07f30c6a07f",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

