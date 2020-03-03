---
title: "deviceManagementComplexSettingInstance resource type"
description: "A setting instance representing a complex value"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementComplexSettingInstance resource type

A setting instance representing a complex value


Inherits from [deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementComplexSettingInstances](../api/devicemanagementcomplexsettinginstance-list.md)|[deviceManagementComplexSettingInstance](../resources/deviceManagementComplexSettingInstance.md) collection|List properties and relationships of the [deviceManagementComplexSettingInstance](../resources/devicemanagementcomplexsettinginstance.md) objects.|
|[Get deviceManagementComplexSettingInstance](../api/devicemanagementcomplexsettinginstance-get.md)|[deviceManagementComplexSettingInstance](../resources/deviceManagementComplexSettingInstance.md)|Read properties and relationships of the [deviceManagementComplexSettingInstance](../resources/devicemanagementcomplexsettinginstance.md) object.|
|[Create deviceManagementComplexSettingInstance](../api/devicemanagementcomplexsettinginstance-create.md)|[deviceManagementComplexSettingInstance](../resources/deviceManagementComplexSettingInstance.md)|Create a new [deviceManagementComplexSettingInstance](../resources/devicemanagementcomplexsettinginstance.md) object.|
|[Delete deviceManagementComplexSettingInstance](../api/devicemanagementcomplexsettinginstance-delete.md)|None|Deletes a [deviceManagementComplexSettingInstance](../resources/devicemanagementcomplexsettinginstance.md).|
|[Update deviceManagementComplexSettingInstance](../api/devicemanagementcomplexsettinginstance-update.md)|[deviceManagementComplexSettingInstance](../resources/deviceManagementComplexSettingInstance.md)|Update the properties of a [deviceManagementComplexSettingInstance](../resources/devicemanagementcomplexsettinginstance.md) object.|
|[List value](../api/devicemanagementcomplexsettinginstance-list-value.md)|[deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md) collection|Get the deviceManagementSettingInstances from the value navigation property.|
|[Create value](../api/devicemanagementcomplexsettinginstance-post-value.md)|[deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)|Create value by posting to the value collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definitionId|String|The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|valueJson|String|JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|value|[deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md) collection|The values that make up the complex setting|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementComplexSettingInstance",
  "baseType": "microsoft.graph.deviceManagementSettingInstance",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```

