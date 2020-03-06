---
title: "deviceAndAppManagementRoleAssignment resource type"
description: "The Role Assignment resource. Role assignments tie together a role definition with members and scopes. There can be one or more role assignments per role. This applies to custom and built-in roles."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceAndAppManagementRoleAssignment resource type


Namespace: microsoft.graph

The Role Assignment resource. Role assignments tie together a role definition with members and scopes. There can be one or more role assignments per role. This applies to custom and built-in roles.


Inherits from [roleAssignment](../resources/roleassignment.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceAndAppManagementRoleAssignment](../api/deviceandappmanagementroleassignment-get.md)|[deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md)|Read properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md) object.|
|[Update deviceAndAppManagementRoleAssignment](../api/deviceandappmanagementroleassignment-update.md)|[deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md)|Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/deviceandappmanagementroleassignment.md) object.|
|[Get roleDefinition](../api/roledefinition-get.md)|[roleDefinition](../resources/roledefinition.md)|Read properties and relationships of the [roleDefinition](../resources/roledefinition.md) object.|
|[List roleScopeTags](../api/deviceandappmanagementroleassignment-list-rolescopetags.md)|[roleScopeTag](../resources/rolescopetag.md) collection|Get the roleScopeTags from the roleScopeTags navigation property.|
|[Create roleScopeTags](../api/deviceandappmanagementroleassignment-post-rolescopetags.md)|[roleScopeTag](../resources/rolescopetag.md)|Create roleScopeTags by posting to the roleScopeTags collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|Description of the Role Assignment. Inherited from [roleAssignment](../resources/roleassignment.md)|
|displayName|String|The display or friendly name of the role Assignment. Inherited from [roleAssignment](../resources/roleassignment.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|members|String collection|The list of ids of role member security groups. These are IDs from Azure Active Directory.|
|resourceScopes|String collection|List of ids of role scope member security groups.  These are IDs from Azure Active Directory. Inherited from [roleAssignment](../resources/roleassignment.md)|
|scopeMembers|String collection|List of ids of role scope member security groups.  These are IDs from Azure Active Directory. Inherited from [roleAssignment](../resources/roleassignment.md)|
|scopeType|Enumeration|Specifies the type of scope for a Role Assignment. Default type 'ResourceScope' allows assignment of ResourceScopes. For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty. Inherited from [roleAssignment](../resources/roleassignment.md). Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/roledefinition.md)|Role definition this assignment is part of. Inherited from [roleAssignment](../resources/roleassignment.md)|
|roleScopeTags|[roleScopeTag](../resources/rolescopetag.md) collection|The set of Role Scope Tags defined on the Role Assignment.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleAssignment",
  "baseType": "microsoft.graph.roleAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String",
  "resourceScopes": [
    "String"
  ],
  "members": [
    "String"
  ]
}
```

