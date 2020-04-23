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
POST /deviceManagement/roleAssignments
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md) object.

The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|The display or friendly name of the role Assignment. Inherited from [roleAssignment](../resources/roleassignment.md)|
|description|String|Description of the Role Assignment. Inherited from [roleAssignment](../resources/roleassignment.md)|
|resourceScopes|String collection|List of ids of role scope member security groups.  These are IDs from Azure Active Directory. Inherited from [roleAssignment](../resources/roleassignment.md)|
|members|String collection|The list of ids of role member security groups. These are IDs from Azure Active Directory.|



## Response
If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_deviceandappmanagementroleassignment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleAssignments
Content-Type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceandappmanagementroleassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "4a262348-2348-4a26-4823-264a4823264a",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

