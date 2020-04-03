---
title: "deviceManagementSettingInstance resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementSettingInstance resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementSettingInstance](../api/devicemanagementsettinginstance-get.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|Read properties and relationships of the [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definitionId|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|valueJson|String||

## Relationships
None

## JSON representation
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

