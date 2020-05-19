---
title: "deviceAndAppManagementRoleAssignment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceAndAppManagementRoleAssignment resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [roleAssignment](../resources/roleassignment.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List roleDefinition](../api/deviceandappmanagementroleassignment-list-roledefinition.md)|[roleDefinition](../resources/intune-roledefinition.md) collection|Get the roleDefinitions from the roleDefinition navigation property.|
|[Add roleDefinition](../api/deviceandappmanagementroleassignment-post-roledefinition.md)|[roleDefinition](../resources/intune-roledefinition.md)|Add roleDefinition by posting to the roleDefinition collection.|
|[Remove roleDefinition](../api/deviceandappmanagementroleassignment-delete-roledefinition.md)|None|Remove a [roleDefinition](../resources/intune-roledefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description** Inherited from [roleAssignment](../resources/intune-roleassignment.md)|
|displayName|String|**TODO: Add Description** Inherited from [roleAssignment](../resources/intune-roleassignment.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|members|String collection|**TODO: Add Description**|
|resourceScopes|String collection|**TODO: Add Description** Inherited from [roleAssignment](../resources/intune-roleassignment.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleDefinition|[roleDefinition](../resources/intune-roledefinition.md)|**TODO: Add Description** Inherited from [roleAssignment](../resources/roleassignment.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementRoleAssignment",
  "baseType": "microsoft.graph.roleAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "resourceScopes": [
    "String"
  ],
  "members": [
    "String"
  ]
}
```

