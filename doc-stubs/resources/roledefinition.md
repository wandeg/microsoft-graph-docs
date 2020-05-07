---
title: "roleDefinition resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# roleDefinition resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List roleAssignments](../api/roledefinition-list-roleassignments.md)|[roleAssignment](../resources/roleassignment.md) collection|Get the roleAssignments from the roleAssignments navigation property.|
|[Create roleAssignments](../api/roledefinition-post-roleassignments.md)|[roleAssignment](../resources/roleassignment.md)|Create a new roleAssignments object.|
|[Delete roleAssignments](../api/roledefinition-delete-roleassignments.md)|None|Delete a [roleAssignment](../resources/roleassignment.md) object.|
|[Update roleAssignments](../api/roledefinition-update-roleassignments.md)|[roleAssignment](../resources/roleassignment.md)|Update the properties of a roleAssignments object.|
|[Get roleAssignment](../api/roleassignment-get.md)|[roleAssignment](../resources/roleassignment.md)|Read the properties and relationships of a [roleAssignment](../resources/roleassignment.md) object.|
|[List roleDefinition](../api/deviceandappmanagementroleassignment-list-roledefinition.md)|[roleDefinition](../resources/roledefinition.md) collection|Get the roleDefinitions from the roleDefinition navigation property.|
|[Add roleDefinition](../api/deviceandappmanagementroleassignment-post-roledefinition.md)|[roleDefinition](../resources/roledefinition.md)|Add roleDefinition by posting to the roleDefinition collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isBuiltIn|Boolean|**TODO: Add Description**|
|isBuiltInRoleDefinition|Boolean|**TODO: Add Description**|
|permissions|[rolePermission](../resources/rolepermission.md) collection|**TODO: Add Description**|
|rolePermissions|[rolePermission](../resources/rolepermission.md) collection|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|roleAssignments|[roleAssignment](../resources/roleassignment.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission"
    }
  ],
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission"
    }
  ],
  "isBuiltInRoleDefinition": "Boolean",
  "isBuiltIn": "Boolean",
  "roleScopeTagIds": [
    "String"
  ]
}
```

