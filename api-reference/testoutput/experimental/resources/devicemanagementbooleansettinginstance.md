---
title: "deviceManagementBooleanSettingInstance resource type"
description: "A setting instance representing a boolean value"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementBooleanSettingInstance resource type

A setting instance representing a boolean value


Inherits from [deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementBooleanSettingInstances](../api/devicemanagementbooleansettinginstance-list.md)|[deviceManagementBooleanSettingInstance](../resources/deviceManagementBooleanSettingInstance.md) collection|List properties and relationships of the [deviceManagementBooleanSettingInstance](../resources/devicemanagementbooleansettinginstance.md) objects.|
|[Get deviceManagementBooleanSettingInstance](../api/devicemanagementbooleansettinginstance-get.md)|[deviceManagementBooleanSettingInstance](../resources/deviceManagementBooleanSettingInstance.md)|Read properties and relationships of the [deviceManagementBooleanSettingInstance](../resources/devicemanagementbooleansettinginstance.md) object.|
|[Create deviceManagementBooleanSettingInstance](../api/devicemanagementbooleansettinginstance-create.md)|[deviceManagementBooleanSettingInstance](../resources/deviceManagementBooleanSettingInstance.md)|Create a new [deviceManagementBooleanSettingInstance](../resources/devicemanagementbooleansettinginstance.md) object.|
|[Delete deviceManagementBooleanSettingInstance](../api/devicemanagementbooleansettinginstance-delete.md)|None|Deletes a [deviceManagementBooleanSettingInstance](../resources/devicemanagementbooleansettinginstance.md).|
|[Update deviceManagementBooleanSettingInstance](../api/devicemanagementbooleansettinginstance-update.md)|[deviceManagementBooleanSettingInstance](../resources/deviceManagementBooleanSettingInstance.md)|Update the properties of a [deviceManagementBooleanSettingInstance](../resources/devicemanagementbooleansettinginstance.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definitionId|String|The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|value|Boolean|The boolean value|
|valueJson|String|JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementBooleanSettingInstance",
  "baseType": "microsoft.graph.deviceManagementSettingInstance",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": true
}
```

