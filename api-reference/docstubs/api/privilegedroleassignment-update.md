---
title: "Update privilegedRoleAssignment"
description: "Update the properties of a privilegedRoleAssignment object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update privilegedRoleAssignment

Namespace: microsoft.graph

Update the properties of a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.

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
PATCH /privilegedRoleAssignments/{privilegedRoleAssignmentsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.

The following table shows the properties that are required when you create the [privilegedRoleAssignment](../resources/privilegedroleassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|userId|String|**TODO: Add Description**|
|roleId|String|**TODO: Add Description**|
|isElevated|Boolean|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|resultMessage|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_privilegedroleassignment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/privilegedRoleAssignments/{privilegedRoleAssignmentsId}
Content-Type: application/json
Content-length: 254

{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignment",
  "userId": "User Id value",
  "roleId": "Role Id value",
  "isElevated": true,
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "resultMessage": "Result Message value"
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
  "@odata.type": "#microsoft.graph.privilegedRoleAssignment",
  "id": "0b252230-2230-0b25-3022-250b3022250b",
  "userId": "User Id value",
  "roleId": "Role Id value",
  "isElevated": true,
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "resultMessage": "Result Message value"
}
```

