---
title: "roleAssignment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# roleAssignment resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List roleAssignments](../api/intune-roledefinition-list-roleassignments.md)|[roleAssignment](../resources/intune-roleassignment.md) collection|Get the roleAssignments from the roleAssignments navigation property.|
|[Create roleAssignments](../api/intune-roledefinition-post-roleassignments.md)|[roleAssignment](../resources/intune-roleassignment.md)|Create a new roleAssignments object.|
|[Delete roleAssignments](../api/intune-roledefinition-delete-roleassignments.md)|None|Delete a [roleAssignment](../resources/intune-roleassignment.md) object.|
|[Update roleAssignments](../api/intune-roledefinition-update-roleassignments.md)|[roleAssignment](../resources/intune-roleassignment.md)|Update the properties of a roleAssignments object.|
|[Get roleAssignments](../api/intune-roledefinition-get-roleassignment.md)|[roleAssignment](../resources/intune-roleassignment.md)|Read the properties and relationships of a [roleAssignment](../resources/intune-roleassignment.md) object.|
|[List roleDefinition](../api/intune-roleassignment-list-roledefinition.md)|[roleDefinition](../resources/intune-roledefinition.md) collection|Get the roleDefinitions from the roleDefinition navigation property.|
|[Add roleDefinition](../api/intune-roleassignment-post-roledefinition.md)|[roleDefinition](../resources/intune-roledefinition.md)|Add roleDefinition by posting to the roleDefinition collection.|
|[Remove roleDefinition](../api/intune-roleassignment-delete-roledefinition.md)|None|Remove a [roleDefinition](../resources/intune-roledefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|resourceScopes|String collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune-roledefinition.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ]
}
```

