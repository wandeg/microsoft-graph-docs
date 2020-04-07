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
|[Get unifiedRoleAssignment](../api/unifiedroleassignment-get.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md)|Read properties and relationships of the [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.|
|[Update unifiedRoleAssignment](../api/unifiedroleassignment-update.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md)|Update the properties of a [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.|
|[Get unifiedRoleDefinition](../api/unifiedroledefinition-get.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Read properties and relationships of the [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.|
|[Get directoryObject](../api/directoryobject-get.md)|[directoryObject](../resources/directoryobject.md)|Read properties and relationships of the [directoryObject](../resources/directoryobject.md) object.|
|[Get directoryObject](../api/directoryobject-get.md)|[directoryObject](../resources/directoryobject.md)|Read properties and relationships of the [directoryObject](../resources/directoryobject.md) object.|
|[Get appScope](../api/appscope-get.md)|[appScope](../resources/appscope.md)|Read properties and relationships of the [appScope](../resources/appscope.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appScopeId|String||
|condition|String||
|directoryScopeId|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|principalId|String||
|resourceScope|String||
|roleDefinitionId|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)||
|directoryScope|[directoryObject](../resources/directoryobject.md)||
|principal|[directoryObject](../resources/directoryobject.md)||
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)||

## JSON representation
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
  "roleDefinitionId": "String",
  "condition": "String",
  "principalId": "String",
  "directoryScopeId": "String",
  "appScopeId": "String",
  "resourceScope": "String"
}
```

