---
title: "deviceAndAppManagementRoleDefinition resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceAndAppManagementRoleDefinition resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [roleDefinition](../resources/roledefinition.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List roleAssignments](../api/deviceandappmanagementroledefinition-list-roleassignments.md)|[roleAssignment](../resources/intune-roleassignment.md) collection|Get the roleAssignments from the roleAssignments navigation property.|
|[Create roleAssignments](../api/deviceandappmanagementroledefinition-post-roleassignments.md)|[roleAssignment](../resources/intune-roleassignment.md)|Create a new roleAssignments object.|
|[Delete roleAssignments](../api/deviceandappmanagementroledefinition-delete-roleassignments.md)|None|Delete a [roleAssignment](../resources/intune-roleassignment.md) object.|
|[Update roleAssignments](../api/deviceandappmanagementroledefinition-update-roleassignments.md)|[roleAssignment](../resources/intune-roleassignment.md)|Update the properties of a roleAssignments object.|
|[Get roleAssignments](../api/deviceandappmanagementroledefinition-get-roleassignment.md)|[roleAssignment](../resources/intune-roleassignment.md)|Read the properties and relationships of a [roleAssignment](../resources/intune-roleassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description** Inherited from [roleDefinition](../resources/intune-roledefinition.md)|
|displayName|String|**TODO: Add Description** Inherited from [roleDefinition](../resources/intune-roledefinition.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isBuiltIn|Boolean|**TODO: Add Description** Inherited from [roleDefinition](../resources/intune-roledefinition.md)|
|rolePermissions|[rolePermission](../resources/intune-rolepermission.md) collection|**TODO: Add Description** Inherited from [roleDefinition](../resources/intune-roledefinition.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleAssignments|[roleAssignment](../resources/intune-roleassignment.md) collection|**TODO: Add Description** Inherited from [roleDefinition](../resources/roledefinition.md)|

## JSON representation
The following is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.rolePermission"
    }
  ],
  "isBuiltIn": "Boolean"
}
```

