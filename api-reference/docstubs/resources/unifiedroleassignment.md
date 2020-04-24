---
title: "unifiedRoleAssignment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# unifiedRoleAssignment resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get unifiedRoleAssignment](../api/unifiedroleassignment-get.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md)|Read the properties and relationships of an [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.|
|[Update unifiedRoleAssignment](../api/unifiedroleassignment-update.md)|[unifiedRoleAssignment](../resources/unifiedroleassignment.md)|Update the properties of an [unifiedRoleAssignment](../resources/unifiedroleassignment.md) object.|
|[List roleDefinition](../api/unifiedroleassignment-list-roledefinition.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection|Get the unifiedRoleDefinitions from the roleDefinition navigation property.|
|[Add roleDefinition](../api/unifiedroleassignment-post-roledefinition.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Add roleDefinition by posting to the roleDefinition collection.|
|[Remove roleDefinition](../api/unifiedroleassignment-delete-roledefinition.md)|None|Remove a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.|
|[List principal](../api/unifiedroleassignment-list-principal.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the principal navigation property.|
|[Add principal](../api/unifiedroleassignment-post-principal.md)|[directoryObject](../resources/directoryobject.md)|Add principal by posting to the principal collection.|
|[Remove principal](../api/unifiedroleassignment-delete-principal.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List directoryScope](../api/unifiedroleassignment-list-directoryscope.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the directoryScope navigation property.|
|[Add directoryScope](../api/unifiedroleassignment-post-directoryscope.md)|[directoryObject](../resources/directoryobject.md)|Add directoryScope by posting to the directoryScope collection.|
|[Remove directoryScope](../api/unifiedroleassignment-delete-directoryscope.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List appScope](../api/unifiedroleassignment-list-appscope.md)|[appScope](../resources/appscope.md) collection|Get the appScopes from the appScope navigation property.|
|[Create appScope](../api/unifiedroleassignment-post-appscope.md)|[appScope](../resources/appscope.md)|Create a new appScope object.|
|[Delete appScope](../api/unifiedroleassignment-delete-appscope.md)|None|Delete an [appScope](../resources/appscope.md) object.|
|[Update appScope](../api/unifiedroleassignment-update-appscope.md)|[appScope](../resources/appscope.md)|Update the properties of an appScope object.|
|[Get appScope](../api/appscope-get.md)|[appScope](../resources/appscope.md)|Read the properties and relationships of an [appScope](../resources/appscope.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appScopeId|String|**TODO: Add Description**|
|condition|String|**TODO: Add Description**|
|directoryScopeId|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|principalId|String|**TODO: Add Description**|
|resourceScope|String|**TODO: Add Description**|
|roleDefinitionId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appScope|[appScope](../resources/appscope.md)|**TODO: Add Description**|
|directoryScope|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|principal|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|**TODO: Add Description**|

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

