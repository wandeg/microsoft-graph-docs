---
title: "Update unifiedRoleAssignment"
description: "Update the properties of a unifiedRoleAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update unifiedRoleAssignment

Namespace: microsoft.graph

Update the properties of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /roleManagement/directory/roleAssignments/{unifiedRoleAssignmentId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.

The following table shows the properties that are required when you create the [unifiedRoleAssignment](../resources/unifiedroleassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|roleDefinitionId|String||
|condition|String||
|principalId|String||
|directoryScopeId|String||
|appScopeId|String||
|resourceScope|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_unifiedroleassignment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/directory/roleAssignments/{unifiedRoleAssignmentId}
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
  "id": "67fdec85-ec85-67fd-85ec-fd6785ecfd67",
  "roleDefinitionId": "Role Definition Id value",
  "condition": "Condition value",
  "principalId": "Principal Id value",
  "directoryScopeId": "Directory Scope Id value",
  "appScopeId": "App Scope Id value",
  "resourceScope": "Resource Scope value"
}
```

