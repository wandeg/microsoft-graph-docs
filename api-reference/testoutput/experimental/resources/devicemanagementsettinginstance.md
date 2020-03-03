---
title: "deviceManagementSettingInstance resource type"
description: "Base type for a setting instance"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementSettingInstance resource type


Namespace: microsoft.graph

Base type for a setting instance


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementSettingInstances](../api/devicemanagementsettinginstance-list.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection|List properties and relationships of the [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) objects.|
|[Get deviceManagementSettingInstance](../api/devicemanagementsettinginstance-get.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|Read properties and relationships of the [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definitionId|String|The ID of the setting definition for this instance|
|id|String| Inherited from [entity](../resources/entity.md)|
|valueJson|String|JSON representation of the value|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingInstance",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```

