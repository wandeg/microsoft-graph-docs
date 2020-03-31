---
title: "rbacApplicationMultiple resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# rbacApplicationMultiple resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get rbacApplicationMultiple](../api/rbacapplicationmultiple-get.md)|[rbacApplicationMultiple](../resources/rbacapplicationmultiple.md)|Read properties and relationships of the [rbacApplicationMultiple](../resources/rbacapplicationmultiple.md) object.|
|[Update rbacApplicationMultiple](../api/rbacapplicationmultiple-update.md)|[rbacApplicationMultiple](../resources/rbacapplicationmultiple.md)|Update the properties of a [rbacApplicationMultiple](../resources/rbacapplicationmultiple.md) object.|
|[List roleDefinitions](../api/rbacapplicationmultiple-list-roledefinitions.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection|Get the unifiedRoleDefinitions from the roleDefinitions navigation property.|
|[Add roleDefinitions](../api/rbacapplicationmultiple-post-roledefinitions.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Add roleDefinitions by posting to the roleDefinitions collection.|
|[List roleAssignments](../api/rbacapplicationmultiple-list-roleassignments.md)|[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) collection|Get the unifiedRoleAssignmentMultiples from the roleAssignments navigation property.|
|[Add roleAssignments](../api/rbacapplicationmultiple-post-roleassignments.md)|[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)|Add roleAssignments by posting to the roleAssignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleAssignments|[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) collection||
|roleDefinitions|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection||

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

