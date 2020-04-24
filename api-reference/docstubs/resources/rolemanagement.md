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


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get roleManagement](../api/rolemanagement-get.md)|[roleManagement](../resources/rolemanagement.md)|Read the properties and relationships of a [roleManagement](../resources/rolemanagement.md) object.|
|[Update roleManagement](../api/rolemanagement-update.md)|[roleManagement](../resources/rolemanagement.md)|Update the properties of a [roleManagement](../resources/rolemanagement.md) object.|
|[List directory](../api/rolemanagement-list-directory.md)|[rbacApplication](../resources/rbacapplication.md) collection|Get the rbacApplications from the directory navigation property.|
|[Create directory](../api/rolemanagement-post-directory.md)|[rbacApplication](../resources/rbacapplication.md)|Create a new directory object.|
|[Delete directory](../api/rolemanagement-delete-directory.md)|None|Delete a [rbacApplication](../resources/rbacapplication.md) object.|
|[Update directory](../api/rolemanagement-update-directory.md)|[rbacApplication](../resources/rbacapplication.md)|Update the properties of a directory object.|
|[Get rbacApplication](../api/rbacapplication-get.md)|[rbacApplication](../resources/rbacapplication.md)|Read the properties and relationships of a [rbacApplication](../resources/rbacapplication.md) object.|
|[List deviceManagement](../api/rolemanagement-list-devicemanagement.md)|[rbacApplicationMultiple](../resources/rbacapplicationmultiple.md) collection|Get the rbacApplicationMultiples from the deviceManagement navigation property.|
|[Create deviceManagement](../api/rolemanagement-post-devicemanagement.md)|[rbacApplicationMultiple](../resources/rbacapplicationmultiple.md)|Create a new deviceManagement object.|
|[Delete deviceManagement](../api/rolemanagement-delete-devicemanagement.md)|None|Delete a [rbacApplicationMultiple](../resources/rbacapplicationmultiple.md) object.|
|[Update deviceManagement](../api/rolemanagement-update-devicemanagement.md)|[rbacApplicationMultiple](../resources/rbacapplicationmultiple.md)|Update the properties of a deviceManagement object.|
|[Get rbacApplicationMultiple](../api/rbacapplicationmultiple-get.md)|[rbacApplicationMultiple](../resources/rbacapplicationmultiple.md)|Read the properties and relationships of a [rbacApplicationMultiple](../resources/rbacapplicationmultiple.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deviceManagement|[rbacApplicationMultiple](../resources/rbacapplicationmultiple.md)|The RbacApplication for Device Management|
|directory|[rbacApplication](../resources/rbacapplication.md)|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
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

