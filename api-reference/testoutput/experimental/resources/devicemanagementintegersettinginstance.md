---
title: "deviceManagementIntegerSettingInstance resource type"
description: "A setting instance representing an integer value"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementIntegerSettingInstance resource type


Namespace: microsoft.graph

A setting instance representing an integer value


Inherits from [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementIntegerSettingInstances](../api/devicemanagementintegersettinginstance-list.md)|[deviceManagementIntegerSettingInstance](../resources/devicemanagementintegersettinginstance.md) collection|List properties and relationships of the [deviceManagementIntegerSettingInstance](../resources/devicemanagementintegersettinginstance.md) objects.|
|[Get deviceManagementIntegerSettingInstance](../api/devicemanagementintegersettinginstance-get.md)|[deviceManagementIntegerSettingInstance](../resources/devicemanagementintegersettinginstance.md)|Read properties and relationships of the [deviceManagementIntegerSettingInstance](../resources/devicemanagementintegersettinginstance.md) object.|
|[Create deviceManagementIntegerSettingInstance](../api/devicemanagementintegersettinginstance-create.md)|[deviceManagementIntegerSettingInstance](../resources/devicemanagementintegersettinginstance.md)|Create a new [deviceManagementIntegerSettingInstance](../resources/devicemanagementintegersettinginstance.md) object.|
|[Delete deviceManagementIntegerSettingInstance](../api/devicemanagementintegersettinginstance-delete.md)|None|Deletes a [deviceManagementIntegerSettingInstance](../resources/devicemanagementintegersettinginstance.md).|
|[Update deviceManagementIntegerSettingInstance](../api/devicemanagementintegersettinginstance-update.md)|[deviceManagementIntegerSettingInstance](../resources/devicemanagementintegersettinginstance.md)|Update the properties of a [deviceManagementIntegerSettingInstance](../resources/devicemanagementintegersettinginstance.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definitionId|String|The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|value|Int32|The integer value|
|valueJson|String|JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntegerSettingInstance",
  "baseType": "microsoft.graph.deviceManagementSettingInstance",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": 1024
}
```

