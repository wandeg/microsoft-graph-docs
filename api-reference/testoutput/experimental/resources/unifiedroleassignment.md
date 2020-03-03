---
title: "unifiedRoleAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# unifiedRoleAssignment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List unifiedRoleAssignments](../api/unifiedroleassignment-list.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md) collection|List properties and relationships of the [unifiedRoleAssignment](../resources/unifiedroleassignment.md) objects.|
|[Get unifiedRoleAssignment](../api/unifiedroleassignment-get.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md)|Read properties and relationships of the [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.|
|[Create unifiedRoleAssignment](../api/unifiedroleassignment-create.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md)|Create a new [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.|
|[Delete unifiedRoleAssignment](../api/unifiedroleassignment-delete.md)|None|Deletes a [unifiedRoleAssignment](../resources/unifiedroleassignment.md).|
|[Update unifiedRoleAssignment](../api/unifiedroleassignment-update.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md)|Update the properties of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.|
|[Get directoryObject](../api/directoryobject-get.md)|[directoryObject](../resources/directoryobject.md)|Read properties and relationships of the [directoryObject](../resources/directoryobject.md) object.|
|[Get unifiedRoleDefinition](../api/unifiedroledefinition-get.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Read properties and relationships of the [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|principalId|String||
|resourceScope|String||
|roleDefinitionId|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|principal|[directoryObject](../resources/directoryobject.md)||
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignment",
  "id": "String (identifier)",
  "principalId": "String",
  "resourceScope": "String",
  "roleDefinitionId": "String"
}
```

