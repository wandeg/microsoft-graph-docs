---
title: "roleManagement resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# roleManagement resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List roleManagements](../api/rolemanagement-list.md)|[roleManagement](../resources/rolemanagement.md) collection|Get a list of the [roleManagement](../resources/rolemanagement.md) objects and their properties.|
|[Create roleManagement](../api/rolemanagement-create.md)|[roleManagement](../resources/rolemanagement.md)|Create a new [roleManagement](../resources/rolemanagement.md) object.|
|[Get roleManagement](../api/rolemanagement-get.md)|[roleManagement](../resources/rolemanagement.md)|Read the properties and relationships of a [roleManagement](../resources/rolemanagement.md) object.|
|[Update roleManagement](../api/rolemanagement-update.md)|[roleManagement](../resources/rolemanagement.md)|Update the properties of a [roleManagement](../resources/rolemanagement.md) object.|
|[Delete roleManagement](../api/rolemanagement-delete.md)|None|Deletes a [roleManagement](../resources/rolemanagement.md) object.|
|[List directory](../api/rolemanagement-list-directory.md)|[rbacApplication](../resources/rbacapplication.md) collection|Get the rbacApplications from the directory navigation property.|
|[Create directory](../api/rolemanagement-post-directory.md)|[rbacApplication](../resources/rbacapplication.md)|Create a new directory object.|
|[Get directory](../api/rolemanagement-get-rbacapplication.md)|[rbacApplication](../resources/rbacapplication.md)|Read the properties and relationships of a [rbacApplication](../resources/rbacapplication.md) object.|
|[Update directory](../api/rolemanagement-update-directory.md)|[rbacApplication](../resources/rbacapplication.md)|Update the properties of a directory object.|
|[Delete directory](../api/rolemanagement-delete-directory.md)|None|Delete a [rbacApplication](../resources/rbacapplication.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|directory|[rbacApplication](../resources/rbacapplication.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleManagement",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleManagement",
  "id": "String (identifier)"
}
```

