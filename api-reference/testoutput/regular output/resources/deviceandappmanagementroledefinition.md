---
title: "deviceAndAppManagementRoleDefinition resource type"
description: "The Role Definition resource. The role definition is the foundation of role based access in Intune. The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource. There are two types of roles, built-in and custom. Built-in roles cannot be modified. Both built-in roles and custom roles must have assignments to be enforced. Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceAndAppManagementRoleDefinition resource type

The Role Definition resource. The role definition is the foundation of role based access in Intune. The role combines an Intune resource such as a Mobile App and associated role permissions such as Create or Read for the resource. There are two types of roles, built-in and custom. Built-in roles cannot be modified. Both built-in roles and custom roles must have assignments to be enforced. Create custom roles if you want to define a role that allows any of the available resources and role permissions to be combined into a single role.


Inherits from [roleDefinition](../resources/roleDefinition.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceAndAppManagementRoleDefinitions](../api/deviceandappmanagementroledefinition-list.md)|[deviceAndAppManagementRoleDefinition](../resources/deviceAndAppManagementRoleDefinition.md) collection|List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/deviceandappmanagementroledefinition.md) objects.|
|[Get deviceAndAppManagementRoleDefinition](../api/deviceandappmanagementroledefinition-get.md)|[deviceAndAppManagementRoleDefinition](../resources/deviceAndAppManagementRoleDefinition.md)|Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/deviceandappmanagementroledefinition.md) object.|
|[Create deviceAndAppManagementRoleDefinition](../api/deviceandappmanagementroledefinition-create.md)|[deviceAndAppManagementRoleDefinition](../resources/deviceAndAppManagementRoleDefinition.md)|Create a new [deviceAndAppManagementRoleDefinition](../resources/deviceandappmanagementroledefinition.md) object.|
|[Delete deviceAndAppManagementRoleDefinition](../api/deviceandappmanagementroledefinition-delete.md)|None|Deletes a [deviceAndAppManagementRoleDefinition](../resources/deviceandappmanagementroledefinition.md).|
|[Update deviceAndAppManagementRoleDefinition](../api/deviceandappmanagementroledefinition-update.md)|[deviceAndAppManagementRoleDefinition](../resources/deviceAndAppManagementRoleDefinition.md)|Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/deviceandappmanagementroledefinition.md) object.|
|[List roleAssignments](../api/deviceandappmanagementroledefinition-list-roleassignments.md)|[roleAssignment](../resources/roleAssignment.md) collection|Get the roleAssignments from the roleAssignments navigation property.|
|[Add roleAssignments](../api/deviceandappmanagementroledefinition-post-roleassignments.md)|[roleAssignment](../resources/roleAssignment.md)|Add roleAssignments by posting to the roleAssignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|Description of the Role definition. Inherited from [roleDefinition](../resources/roleDefinition.md)|
|displayName|String|Display Name of the Role definition. Inherited from [roleDefinition](../resources/roleDefinition.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isBuiltIn|Boolean|Type of Role. Set to True if it is built-in, or set to False if it is a custom role definition. Inherited from [roleDefinition](../resources/roleDefinition.md)|
|rolePermissions|[rolePermission](../resources/rolePermission.md) collection|List of Role Permissions this role is allowed to perform. These must match the actionName that is defined as part of the rolePermission. Inherited from [roleDefinition](../resources/roleDefinition.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleAssignments|[roleAssignment](../resources/roleAssignment.md) collection|List of Role assignments for this role definition. Inherited from [roleDefinition](../resources/roleDefinition.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleDefinition",
  "baseType": "microsoft.graph.roleDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "String"
          ],
          "notAllowedResourceActions": [
            "String"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```

