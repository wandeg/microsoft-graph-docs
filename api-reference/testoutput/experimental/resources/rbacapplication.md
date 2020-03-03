---
title: "rbacApplication resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# rbacApplication resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List rbacApplications](../api/rbacapplication-list.md)|[rbacApplication](../resources/rbacApplication.md) collection|List properties and relationships of the [rbacApplication](../resources/rbacapplication.md) objects.|
|[Get rbacApplication](../api/rbacapplication-get.md)|[rbacApplication](../resources/rbacApplication.md)|Read properties and relationships of the [rbacApplication](../resources/rbacapplication.md) object.|
|[Create rbacApplication](../api/rbacapplication-create.md)|[rbacApplication](../resources/rbacApplication.md)|Create a new [rbacApplication](../resources/rbacapplication.md) object.|
|[Delete rbacApplication](../api/rbacapplication-delete.md)|None|Deletes a [rbacApplication](../resources/rbacapplication.md).|
|[Update rbacApplication](../api/rbacapplication-update.md)|[rbacApplication](../resources/rbacApplication.md)|Update the properties of a [rbacApplication](../resources/rbacapplication.md) object.|
|[List roleDefinitions](../api/rbacapplication-list-roledefinitions.md)|[unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) collection|Get the unifiedRoleDefinitions from the roleDefinitions navigation property.|
|[Add roleDefinitions](../api/rbacapplication-post-roledefinitions.md)|[unifiedRoleDefinition](../resources/unifiedRoleDefinition.md)|Add roleDefinitions by posting to the roleDefinitions collection.|
|[List roleAssignments](../api/rbacapplication-list-roleassignments.md)|[unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) collection|Get the unifiedRoleAssignments from the roleAssignments navigation property.|
|[Add roleAssignments](../api/rbacapplication-post-roleassignments.md)|[unifiedRoleAssignment](../resources/unifiedRoleAssignment.md)|Add roleAssignments by posting to the roleAssignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleAssignments|[unifiedRoleAssignment](../resources/unifiedRoleAssignment.md) collection||
|roleDefinitions|[unifiedRoleDefinition](../resources/unifiedRoleDefinition.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
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

