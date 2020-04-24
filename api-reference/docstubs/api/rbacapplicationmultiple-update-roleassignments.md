---
title: "Update roleAssignments"
description: "Update the properties of a roleAssignments object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update roleAssignments

Namespace: microsoft.graph

Update the properties of a roleAssignments object.

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
PATCH /roleManagement/deviceManagement/roleAssignments
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.

The following table shows the properties that are required when you create the [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|roleDefinitionId|String|**TODO: Add Description**|
|condition|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|principalIds|String collection|**TODO: Add Description**|
|directoryScopeIds|String collection|**TODO: Add Description**|
|appScopeIds|String collection|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_roleassignments"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/roleManagement/deviceManagement/roleAssignments
Content-Type: application/json
Content-length: 408

{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
  "roleDefinitionId": "Role Definition Id value",
  "condition": "Condition value",
  "displayName": "Display Name value",
  "description": "Description value",
  "principalIds": [
    "Principal Ids value"
  ],
  "directoryScopeIds": [
    "Directory Scope Ids value"
  ],
  "appScopeIds": [
    "App Scope Ids value"
  ]
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
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
  "id": "9f914fa3-4fa3-9f91-a34f-919fa34f919f",
  "roleDefinitionId": "Role Definition Id value",
  "condition": "Condition value",
  "displayName": "Display Name value",
  "description": "Description value",
  "principalIds": [
    "Principal Ids value"
  ],
  "directoryScopeIds": [
    "Directory Scope Ids value"
  ],
  "appScopeIds": [
    "App Scope Ids value"
  ]
}
```

