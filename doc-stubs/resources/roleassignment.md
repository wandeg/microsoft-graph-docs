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
|[List roleDefinition](../api/roleassignment-list-roledefinition.md)|[roleDefinition](../resources/roledefinition.md) collection|Get the roleDefinitions from the roleDefinition navigation property.|
|[Add roleDefinition](../api/roleassignment-post-roledefinition.md)|[roleDefinition](../resources/roledefinition.md)|Add roleDefinition by posting to the roleDefinition collection.|
|[Remove roleDefinition](../api/roleassignment-delete-roledefinition.md)|None|Remove a [roleDefinition](../resources/roledefinition.md) object.|
|[List roleAssignments](../api/roledefinition-list-roleassignments.md)|[roleAssignment](../resources/roleassignment.md) collection|Get the roleAssignments from the roleAssignments navigation property.|
|[Create roleAssignments](../api/roledefinition-post-roleassignments.md)|[roleAssignment](../resources/roleassignment.md)|Create a new roleAssignments object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|resourceScopes|String collection|**TODO: Add Description**|
|scopeMembers|String collection|**TODO: Add Description**|
|scopeType|roleAssignmentScopeType|**TODO: Add Description**. Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/roledefinition.md)|**TODO: Add Description**|

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
  "scopeMembers": [
    "String"
  ],
  "scopeType": "String",
  "resourceScopes": [
    "String"
  ]
}
```

