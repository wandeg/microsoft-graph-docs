---
title: "roleDefinition resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# roleDefinition resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List roleDefinition](../api/deviceandappmanagementroleassignment-list-roledefinition.md)|[roleDefinition](../resources/intune-roledefinition.md) collection|Get the roleDefinitions from the roleDefinition navigation property.|
|[Add roleDefinition](../api/deviceandappmanagementroleassignment-post-roledefinition.md)|[roleDefinition](../resources/intune-roledefinition.md)|Add roleDefinition by posting to the roleDefinition collection.|
|[Remove roleDefinition](../api/deviceandappmanagementroleassignment-delete-roledefinition.md)|None|Remove a [roleDefinition](../resources/intune-roledefinition.md) object.|
|[List roleAssignments](../api/intune-roledefinition-list-roleassignments.md)|[roleAssignment](../resources/intune-roleassignment.md) collection|Get the roleAssignments from the roleAssignments navigation property.|
|[Create roleAssignments](../api/intune-roledefinition-post-roleassignments.md)|[roleAssignment](../resources/intune-roleassignment.md)|Create a new roleAssignments object.|
|[Delete roleAssignments](../api/intune-roledefinition-delete-roleassignments.md)|None|Delete a [roleAssignment](../resources/intune-roleassignment.md) object.|
|[Update roleAssignments](../api/intune-roledefinition-update-roleassignments.md)|[roleAssignment](../resources/intune-roleassignment.md)|Update the properties of a roleAssignments object.|
|[Get roleAssignments](../api/intune-roledefinition-get-roleassignment.md)|[roleAssignment](../resources/intune-roleassignment.md)|Read the properties and relationships of a [roleAssignment](../resources/intune-roleassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isBuiltIn|Boolean|**TODO: Add Description**|
|rolePermissions|[rolePermission](../resources/intune-rolepermission.md) collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleAssignments|[roleAssignment](../resources/intune-roleassignment.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
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

