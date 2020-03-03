---
title: "deviceManagementStringSettingInstance resource type"
description: "A setting instance representing a string value"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementStringSettingInstance resource type

A setting instance representing a string value


Inherits from [deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementStringSettingInstances](../api/devicemanagementstringsettinginstance-list.md)|[deviceManagementStringSettingInstance](../resources/deviceManagementStringSettingInstance.md) collection|List properties and relationships of the [deviceManagementStringSettingInstance](../resources/devicemanagementstringsettinginstance.md) objects.|
|[Get deviceManagementStringSettingInstance](../api/devicemanagementstringsettinginstance-get.md)|[deviceManagementStringSettingInstance](../resources/deviceManagementStringSettingInstance.md)|Read properties and relationships of the [deviceManagementStringSettingInstance](../resources/devicemanagementstringsettinginstance.md) object.|
|[Create deviceManagementStringSettingInstance](../api/devicemanagementstringsettinginstance-create.md)|[deviceManagementStringSettingInstance](../resources/deviceManagementStringSettingInstance.md)|Create a new [deviceManagementStringSettingInstance](../resources/devicemanagementstringsettinginstance.md) object.|
|[Delete deviceManagementStringSettingInstance](../api/devicemanagementstringsettinginstance-delete.md)|None|Deletes a [deviceManagementStringSettingInstance](../resources/devicemanagementstringsettinginstance.md).|
|[Update deviceManagementStringSettingInstance](../api/devicemanagementstringsettinginstance-update.md)|[deviceManagementStringSettingInstance](../resources/deviceManagementStringSettingInstance.md)|Update the properties of a [deviceManagementStringSettingInstance](../resources/devicemanagementstringsettinginstance.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definitionId|String|The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|value|String|The string value|
|valueJson|String|JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementStringSettingInstance",
  "baseType": "microsoft.graph.deviceManagementSettingInstance",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": "String"
}
```

