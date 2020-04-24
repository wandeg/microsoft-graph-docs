---
title: "Create roleAssignments"
description: "Create a new roleAssignments object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create roleAssignments

Namespace: microsoft.graph

Create a new roleAssignments object.

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
POST /roleManagement/directory/roleAssignments
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.

The following table shows the properties that are required when you create the [unifiedRoleAssignment](../resources/unifiedroleassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|roleDefinitionId|String|**TODO: Add Description**|
|condition|String|**TODO: Add Description**|
|principalId|String|**TODO: Add Description**|
|directoryScopeId|String|**TODO: Add Description**|
|appScopeId|String|**TODO: Add Description**|
|resourceScope|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_unifiedroleassignment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments
Content-Type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
  "roleDefinitionId": "Role Definition Id value",
  "condition": "Condition value",
  "principalId": "Principal Id value",
  "directoryScopeId": "Directory Scope Id value",
  "appScopeId": "App Scope Id value",
  "resourceScope": "Resource Scope value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedroleassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
  "id": "9a9af9d0-f9d0-9a9a-d0f9-9a9ad0f99a9a",
  "roleDefinitionId": "Role Definition Id value",
  "condition": "Condition value",
  "principalId": "Principal Id value",
  "directoryScopeId": "Directory Scope Id value",
  "appScopeId": "App Scope Id value",
  "resourceScope": "Resource Scope value"
}
```

