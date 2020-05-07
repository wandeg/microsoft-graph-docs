---
title: "Add roleDefinition"
description: "Add roleDefinition by posting to the roleDefinition collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add roleDefinition

Namespace: microsoft.graph

Add roleDefinition by posting to the roleDefinition collection.

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
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [roleDefinition](../resources/roledefinition.md) object.

The following table shows the properties that are required when you create the [roleDefinition](../resources/roledefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|permissions|[rolePermission](../resources/rolepermission.md) collection|**TODO: Add Description**|
|rolePermissions|[rolePermission](../resources/rolepermission.md) collection|**TODO: Add Description**|
|isBuiltInRoleDefinition|Boolean|**TODO: Add Description**|
|isBuiltIn|Boolean|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|



## Response

If successful, this method returns a `204 No Content` response code and a [roleDefinition](../resources/roledefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_roledefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition/$ref
Content-Type: application/json
Content-length: 418

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "displayName": "String",
  "description": "String",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission"
    }
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission"
    }
  ],
  "isBuiltInRoleDefinition": "Boolean",
  "isBuiltIn": "Boolean",
  "roleScopeTagIds": [
    "String"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.roledefinition"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "2c85dd86-dd86-2c85-86dd-852c86dd852c",
  "displayName": "String",
  "description": "String",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission"
    }
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission"
    }
  ],
  "isBuiltInRoleDefinition": "Boolean",
  "isBuiltIn": "Boolean",
  "roleScopeTagIds": [
    "String"
  ]
}
```

