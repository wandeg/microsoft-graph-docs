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
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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
Content-length: 240

{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
  "roleDefinitionId": "String",
  "condition": "String",
  "principalId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "resourceScope": "String"
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
  "id": "322422a4-22a4-3224-a422-2432a4222432",
  "roleDefinitionId": "String",
  "condition": "String",
  "principalId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "resourceScope": "String"
}
```

