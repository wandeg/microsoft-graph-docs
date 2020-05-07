---
title: "rbacApplication resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# rbacApplication resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List roleDefinitions](../api/rbacapplication-list-roledefinitions.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection|Get the unifiedRoleDefinitions from the roleDefinitions navigation property.|
|[Create roleDefinitions](../api/rbacapplication-post-roledefinitions.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Create a new roleDefinitions object.|
|[Delete roleDefinitions](../api/rbacapplication-delete-roledefinitions.md)|None|Delete a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.|
|[Update roleDefinitions](../api/rbacapplication-update-roledefinitions.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Update the properties of a roleDefinitions object.|
|[Get unifiedRoleDefinition](../api/unifiedroledefinition-get.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Read the properties and relationships of an [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.|
|[List roleAssignments](../api/rbacapplication-list-roleassignments.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md) collection|Get the unifiedRoleAssignments from the roleAssignments navigation property.|
|[Create roleAssignments](../api/rbacapplication-post-roleassignments.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md)|Create a new roleAssignments object.|
|[Delete roleAssignments](../api/rbacapplication-delete-roleassignments.md)|None|Delete a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.|
|[Update roleAssignments](../api/rbacapplication-update-roleassignments.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md)|Update the properties of a roleAssignments object.|
|[Get unifiedRoleAssignment](../api/unifiedroleassignment-get.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md)|Read the properties and relationships of an [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleAssignments|[unifiedRoleAssignment](../resources/unifiedroleassignment.md) collection|**TODO: Add Description**|
|roleDefinitions|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.rbacApplication",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rbacApplication",
  "id": "String (identifier)"
}
```

