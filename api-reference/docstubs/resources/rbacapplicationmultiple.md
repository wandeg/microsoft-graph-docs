---
title: "rbacApplicationMultiple resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# rbacApplicationMultiple resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get rbacApplicationMultiple](../api/rbacapplicationmultiple-get.md)|[rbacApplicationMultiple](../resources/rbacapplicationmultiple.md)|Read the properties and relationships of a [rbacApplicationMultiple](../resources/rbacapplicationmultiple.md) object.|
|[Update rbacApplicationMultiple](../api/rbacapplicationmultiple-update.md)|[rbacApplicationMultiple](../resources/rbacapplicationmultiple.md)|Update the properties of a [rbacApplicationMultiple](../resources/rbacapplicationmultiple.md) object.|
|[List roleDefinitions](../api/rbacapplicationmultiple-list-roledefinitions.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection|Get the unifiedRoleDefinitions from the roleDefinitions navigation property.|
|[Create roleDefinitions](../api/rbacapplicationmultiple-post-roledefinitions.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Create a new roleDefinitions object.|
|[Delete roleDefinitions](../api/rbacapplicationmultiple-delete-roledefinitions.md)|None|Delete a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.|
|[Update roleDefinitions](../api/rbacapplicationmultiple-update-roledefinitions.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Update the properties of a roleDefinitions object.|
|[Get unifiedRoleDefinition](../api/unifiedroledefinition-get.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Read the properties and relationships of an [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.|
|[List roleAssignments](../api/rbacapplicationmultiple-list-roleassignments.md)|[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) collection|Get the unifiedRoleAssignmentMultiples from the roleAssignments navigation property.|
|[Create roleAssignments](../api/rbacapplicationmultiple-post-roleassignments.md)|[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)|Create a new roleAssignments object.|
|[Delete roleAssignments](../api/rbacapplicationmultiple-delete-roleassignments.md)|None|Delete a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.|
|[Update roleAssignments](../api/rbacapplicationmultiple-update-roleassignments.md)|[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)|Update the properties of a roleAssignments object.|
|[Get unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-get.md)|[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)|Read the properties and relationships of an [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleAssignments|[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) collection|**TODO: Add Description**|
|roleDefinitions|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.rbacApplicationMultiple",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rbacApplicationMultiple",
  "id": "String (identifier)"
}
```

