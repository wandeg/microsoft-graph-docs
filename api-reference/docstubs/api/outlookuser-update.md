---
title: "Update outlookUser"
description: "Update the properties of an outlookUser object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update outlookUser

Namespace: microsoft.graph

Update the properties of an [outlookUser](../resources/outlookuser.md) object.

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
PATCH /me/outlook
PATCH /users/{usersId}/outlook
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [outlookUser](../resources/outlookuser.md) object.

The following table shows the properties that are required when you create the [outlookUser](../resources/outlookuser.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [outlookUser](../resources/outlookuser.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_outlookuser"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/outlook
Content-Type: application/json
Content-length: 53

{
  "@odata.type": "#microsoft.graph.outlookUser"
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
  "@odata.type": "#microsoft.graph.outlookUser",
  "id": "f4e56d5d-6d5d-f4e5-5d6d-e5f45d6de5f4"
}
```

