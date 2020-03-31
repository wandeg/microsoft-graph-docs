---
title: "roleManagement resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# roleManagement resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get roleManagement](../api/rolemanagement-get.md)|[roleManagement](../resources/rolemanagement.md)|Read properties and relationships of the [roleManagement](../resources/rolemanagement.md) object.|
|[Update roleManagement](../api/rolemanagement-update.md)|[roleManagement](../resources/rolemanagement.md)|Update the properties of a [roleManagement](../resources/rolemanagement.md) object.|
|[Get rbacApplication](../api/rbacapplication-get.md)|[rbacApplication](../resources/rbacapplication.md)|Read properties and relationships of the [rbacApplication](../resources/rbacapplication.md) object.|
|[Get rbacApplicationMultiple](../api/rbacapplicationmultiple-get.md)|[rbacApplicationMultiple](../resources/rbacapplicationmultiple.md)|Read properties and relationships of the [rbacApplicationMultiple](../resources/rbacapplicationmultiple.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deviceManagement|[rbacApplicationMultiple](../resources/rbacapplicationmultiple.md)||
|directory|[rbacApplication](../resources/rbacapplication.md)||

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

