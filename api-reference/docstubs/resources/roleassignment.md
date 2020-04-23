---
title: "roleAssignment resource type"
description: "The Role Assignment resource. Role assignments tie together a role definition with members and scopes. There can be one or more role assignments per role. This applies to custom and built-in roles."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# roleAssignment resource type


Namespace: microsoft.graph

The Role Assignment resource. Role assignments tie together a role definition with members and scopes. There can be one or more role assignments per role. This applies to custom and built-in roles.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get roleAssignment](../api/roleassignment-get.md)|[roleAssignment](../resources/roleassignment.md)|Read the properties and relationships of a [roleAssignment](../resources/roleassignment.md) object.|
|[Update roleAssignment](../api/roleassignment-update.md)|[roleAssignment](../resources/roleassignment.md)|Update the properties of a [roleAssignment](../resources/roleassignment.md) object.|
|[List roleDefinition](../api/roleassignment-list-roledefinition.md)|[roleDefinition](../resources/roledefinition.md) collection|Get the roleDefinitions from the roleDefinition navigation property.|
|[Add roleDefinition](../api/roleassignment-post-roledefinition.md)|[roleDefinition](../resources/roledefinition.md)|Add roleDefinition by posting to the roleDefinition collection.|
|[Remove roleDefinition](../api/roleassignment-delete-roledefinition.md)|None|Remove a [roleDefinition](../resources/roledefinition.md) object.|
|[List roleAssignments](../api/roledefinition-list-roleassignments.md)|[roleAssignment](../resources/roleassignment.md) collection|Get the roleAssignments from the roleAssignments navigation property.|
|[Create roleAssignments](../api/roledefinition-post-roleassignments.md)|[roleAssignment](../resources/roleassignment.md)|Create a new roleAssignments object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|Description of the Role Assignment.|
|displayName|String|The display or friendly name of the role Assignment.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|resourceScopes|String collection|List of ids of role scope member security groups.  These are IDs from Azure Active Directory.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/roledefinition.md)|Role definition this assignment is part of.|

## JSON representation
Here is a JSON representation of the resource.
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

