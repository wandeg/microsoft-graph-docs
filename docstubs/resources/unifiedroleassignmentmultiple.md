---
title: "unifiedRoleAssignmentMultiple resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# unifiedRoleAssignmentMultiple resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-get.md)|[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)|Read properties and relationships of the [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.|
|[Update unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-update.md)|[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)|Update the properties of a [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.|
|[Get unifiedRoleDefinition](../api/unifiedroledefinition-get.md)|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|Read properties and relationships of the [unifiedRoleDefinition](../resources/unifiedroledefinition.md) object.|
|[List principals](../api/unifiedroleassignmentmultiple-list-principals.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the principals navigation property.|
|[Create principals](../api/unifiedroleassignmentmultiple-post-principals.md)|[directoryObject](../resources/directoryobject.md)|Create principals by posting to the principals collection.|
|[List directoryScopes](../api/unifiedroleassignmentmultiple-list-directoryscopes.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the directoryScopes navigation property.|
|[Create directoryScopes](../api/unifiedroleassignmentmultiple-post-directoryscopes.md)|[directoryObject](../resources/directoryobject.md)|Create directoryScopes by posting to the directoryScopes collection.|
|[List appScopes](../api/unifiedroleassignmentmultiple-list-appscopes.md)|[appScope](../resources/appscope.md) collection|Get the appScopes from the appScopes navigation property.|
|[Add appScopes](../api/unifiedroleassignmentmultiple-post-appscopes.md)|[appScope](../resources/appscope.md)|Add appScopes by posting to the appScopes collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appScopeIds|String collection||
|condition|String||
|description|String||
|directoryScopeIds|String collection||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|principalIds|String collection||
|roleDefinitionId|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appScopes|[appScope](../resources/appscope.md) collection||
|directoryScopes|[directoryObject](../resources/directoryobject.md) collection||
|principals|[directoryObject](../resources/directoryobject.md) collection||
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)||

## JSON representation
Here is a JSON representation of the resource.
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

