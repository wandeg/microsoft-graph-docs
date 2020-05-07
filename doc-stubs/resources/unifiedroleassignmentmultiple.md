---
title: "unifiedRoleAssignmentMultiple resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# unifiedRoleAssignmentMultiple resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List roleDefinition](../api/unifiedroleassignmentmultiple-list-roledefinition.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md) collection|Get the unifiedRoleDefinitions from the roleDefinition navigation property.|
|[Add roleDefinition](../api/unifiedroleassignmentmultiple-post-roledefinition.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Add roleDefinition by posting to the roleDefinition collection.|
|[Remove roleDefinition](../api/unifiedroleassignmentmultiple-delete-roledefinition.md)|None|Remove a [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.|
|[List principals](../api/unifiedroleassignmentmultiple-list-principals.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the principals navigation property.|
|[Add principals](../api/unifiedroleassignmentmultiple-post-principals.md)|[directoryObject](../resources/directoryobject.md)|Add principals by posting to the principals collection.|
|[Remove principals](../api/unifiedroleassignmentmultiple-delete-principals.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List directoryScopes](../api/unifiedroleassignmentmultiple-list-directoryscopes.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the directoryScopes navigation property.|
|[Add directoryScopes](../api/unifiedroleassignmentmultiple-post-directoryscopes.md)|[directoryObject](../resources/directoryobject.md)|Add directoryScopes by posting to the directoryScopes collection.|
|[Remove directoryScopes](../api/unifiedroleassignmentmultiple-delete-directoryscopes.md)|None|Remove a [directoryObject](../resources/directoryobject.md) object.|
|[List appScopes](../api/unifiedroleassignmentmultiple-list-appscopes.md)|[appScope](../resources/appscope.md) collection|Get the appScopes from the appScopes navigation property.|
|[Create appScopes](../api/unifiedroleassignmentmultiple-post-appscopes.md)|[appScope](../resources/appscope.md)|Create a new appScopes object.|
|[Delete appScopes](../api/unifiedroleassignmentmultiple-delete-appscopes.md)|None|Delete an [appScope](../resources/appscope.md) object.|
|[Update appScopes](../api/unifiedroleassignmentmultiple-update-appscopes.md)|[appScope](../resources/appscope.md)|Update the properties of an appScopes object.|
|[Get appScope](../api/appscope-get.md)|[appScope](../resources/appscope.md)|Read the properties and relationships of an [appScope](../resources/appscope.md) object.|
|[List roleAssignments](../api/rbacapplicationmultiple-list-roleassignments.md)|[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) collection|Get the unifiedRoleAssignmentMultiples from the roleAssignments navigation property.|
|[Create roleAssignments](../api/rbacapplicationmultiple-post-roleassignments.md)|[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)|Create a new roleAssignments object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appScopeIds|String collection|**TODO: Add Description**|
|condition|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|directoryScopeIds|String collection|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|principalIds|String collection|**TODO: Add Description**|
|roleDefinitionId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appScopes|[appScope](../resources/appscope.md) collection|**TODO: Add Description**|
|directoryScopes|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|principals|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
  "id": "String (identifier)",
  "roleDefinitionId": "String",
  "condition": "String",
  "displayName": "String",
  "description": "String",
  "principalIds": [
    "String"
  ],
  "directoryScopeIds": [
    "String"
  ],
  "appScopeIds": [
    "String"
  ]
}
```

