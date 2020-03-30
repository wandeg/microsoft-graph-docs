---
title: "roleAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# roleAssignment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get roleAssignment](../api/roleassignment-get.md)|[roleAssignment](../resources/roleassignment.md)|Read properties and relationships of the [roleAssignment](../resources/roleassignment.md) object.|
|[Update roleAssignment](../api/roleassignment-update.md)|[roleAssignment](../resources/roleassignment.md)|Update the properties of a [roleAssignment](../resources/roleassignment.md) object.|
|[Get roleDefinition](../api/roledefinition-get.md)|[roleDefinition](../resources/roledefinition.md)|Read properties and relationships of the [roleDefinition](../resources/roledefinition.md) object.|
|[List roleAssignments](../api/roledefinition-list-roleassignments.md)|[roleAssignment](../resources/roleassignment.md) collection|Get the roleAssignments from the roleAssignments navigation property.|
|[Add roleAssignments](../api/roledefinition-post-roleassignments.md)|[roleAssignment](../resources/roleassignment.md)|Add roleAssignments by posting to the roleAssignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|resourceScopes|String collection||
|scopeMembers|String collection||
|scopeType|Enumeration| Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/roledefinition.md)||

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
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String",
  "resourceScopes": [
    "String"
  ]
}
```

