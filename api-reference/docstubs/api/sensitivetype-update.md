---
title: "Update sensitiveType"
description: "Update the properties of a sensitiveType object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update sensitiveType

Namespace: microsoft.graph

Update the properties of a [sensitiveType](../resources/sensitivetype.md) object.

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
PATCH /dataClassification/sensitiveTypes/{sensitiveTypeId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [sensitiveType](../resources/sensitivetype.md) object.

The following table shows the properties that are required when you create the [sensitiveType](../resources/sensitivetype.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|rulePackageId|String|**TODO: Add Description**|
|rulePackageType|String|**TODO: Add Description**|
|publisherName|String|**TODO: Add Description**|
|state|String|**TODO: Add Description**|
|scope|sensitiveTypeScope|**TODO: Add Description**. Possible values are: `fullDocument`, `partialDocument`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [sensitiveType](../resources/sensitivetype.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_sensitivetype"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/dataClassification/sensitiveTypes/{sensitiveTypeId}
Content-Type: application/json
Content-length: 306

{
  "@odata.type": "#microsoft.graph.sensitiveType",
  "name": "Name value",
  "description": "Description value",
  "rulePackageId": "Rule Package Id value",
  "rulePackageType": "Rule Package Type value",
  "publisherName": "Publisher Name value",
  "state": "State value",
  "scope": "String"
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
  "@odata.type": "#microsoft.graph.sensitiveType",
  "id": "1fdf7c8f-7c8f-1fdf-8f7c-df1f8f7cdf1f",
  "name": "Name value",
  "description": "Description value",
  "rulePackageId": "Rule Package Id value",
  "rulePackageType": "Rule Package Type value",
  "publisherName": "Publisher Name value",
  "state": "State value",
  "scope": "String"
}
```

