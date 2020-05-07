---
title: "Create privilegedRoleAssignment"
description: "Create a new privilegedRoleAssignment object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create privilegedRoleAssignment

Namespace: microsoft.graph

Create a new [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.

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
POST /privilegedRoleAssignments
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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

If successful, this method returns a `201 Created` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignment_from_privilegedroleassignments"
}
-->
``` http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments
Content-Type: application/json
Content-length: 217

{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignment",
  "userId": "String",
  "roleId": "String",
  "isElevated": "Boolean",
  "expirationDateTime": "String (timestamp)",
  "resultMessage": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedroleassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.privilegedRoleAssignment",
  "id": "ee16f899-f899-ee16-99f8-16ee99f816ee",
  "userId": "String",
  "roleId": "String",
  "isElevated": "Boolean",
  "expirationDateTime": "String (timestamp)",
  "resultMessage": "String"
}
```

