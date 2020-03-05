---
title: "roleAssignment resource type"
description: "The Role Assignment resource. Role assignments tie together a role definition with members and scopes. There can be one or more role assignments per role. This applies to custom and built-in roles."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# roleAssignment resource type


Namespace: microsoft.graph

The Role Assignment resource. Role assignments tie together a role definition with members and scopes. There can be one or more role assignments per role. This applies to custom and built-in roles.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List roleAssignments](../api/roleassignment-list.md)|[roleAssignment](../resources/roleassignment.md) collection|List properties and relationships of the [roleAssignment](../resources/roleassignment.md) objects.|
|[Get roleAssignment](../api/roleassignment-get.md)|[roleAssignment](../resources/roleassignment.md)|Read properties and relationships of the [roleAssignment](../resources/roleassignment.md) object.|
|[Create roleAssignment](../api/roleassignment-create.md)|[roleAssignment](../resources/roleassignment.md)|Create a new [roleAssignment](../resources/roleassignment.md) object.|
|[Delete roleAssignment](../api/roleassignment-delete.md)|None|Deletes a [roleAssignment](../resources/roleassignment.md).|
|[Update roleAssignment](../api/roleassignment-update.md)|[roleAssignment](../resources/roleassignment.md)|Update the properties of a [roleAssignment](../resources/roleassignment.md) object.|
|[Get roleDefinition](../api/roledefinition-get.md)|[roleDefinition](../resources/roledefinition.md)|Read properties and relationships of the [roleDefinition](../resources/roledefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|Description of the Role Assignment.|
|displayName|String|The display or friendly name of the role Assignment.|
|id|String| Inherited from [entity](../resources/entity.md)|
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

