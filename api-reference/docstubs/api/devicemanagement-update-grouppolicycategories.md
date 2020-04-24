---
title: "Update groupPolicyCategories"
description: "Update the properties of a groupPolicyCategories object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update groupPolicyCategories

Namespace: microsoft.graph

Update the properties of a groupPolicyCategories object.

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
PATCH /deviceManagement/groupPolicyCategories
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [groupPolicyCategory](../resources/grouppolicycategory.md) object.

The following table shows the properties that are required when you create the [groupPolicyCategory](../resources/grouppolicycategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|The string id of the category's display name|
|isRoot|Boolean|Defines if the category is a root category|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified.|



## Response
If successful, this method returns a `200 OK` response code and an updated [groupPolicyCategory](../resources/grouppolicycategory.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_grouppolicycategories"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyCategories
Content-Type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "displayName": "Display Name value",
  "isRoot": true
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
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "id": "b2cef283-f283-b2ce-83f2-ceb283f2ceb2",
  "displayName": "Display Name value",
  "isRoot": true,
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
}
```

