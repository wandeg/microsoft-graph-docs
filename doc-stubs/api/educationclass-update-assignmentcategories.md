---
title: "Update assignmentCategories"
description: "Update the properties of an assignmentCategories object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update assignmentCategories

Namespace: microsoft.graph

Update the properties of an assignmentCategories object.

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
PATCH /education/classes/{educationClassId}/assignmentCategories
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [educationCategory](../resources/educationcategory.md) object.

The following table shows the properties that are required when you create the [educationCategory](../resources/educationcategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [educationCategory](../resources/educationcategory.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_assignmentcategories"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignmentCategories
Content-Type: application/json
Content-length: 87

{
  "@odata.type": "#microsoft.graph.educationCategory",
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
  "@odata.type": "#microsoft.graph.educationCategory",
  "id": "46ab7696-7696-46ab-9676-ab469676ab46",
  "displayName": "String"
}
```

