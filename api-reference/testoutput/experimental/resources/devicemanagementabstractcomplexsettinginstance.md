---
title: "deviceManagementAbstractComplexSettingInstance resource type"
description: "A setting instance representing a complex value for an abstract setting"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementAbstractComplexSettingInstance resource type

A setting instance representing a complex value for an abstract setting


Inherits from [deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementAbstractComplexSettingInstances](../api/devicemanagementabstractcomplexsettinginstance-list.md)|[deviceManagementAbstractComplexSettingInstance](../resources/deviceManagementAbstractComplexSettingInstance.md) collection|List properties and relationships of the [deviceManagementAbstractComplexSettingInstance](../resources/devicemanagementabstractcomplexsettinginstance.md) objects.|
|[Get deviceManagementAbstractComplexSettingInstance](../api/devicemanagementabstractcomplexsettinginstance-get.md)|[deviceManagementAbstractComplexSettingInstance](../resources/deviceManagementAbstractComplexSettingInstance.md)|Read properties and relationships of the [deviceManagementAbstractComplexSettingInstance](../resources/devicemanagementabstractcomplexsettinginstance.md) object.|
|[Create deviceManagementAbstractComplexSettingInstance](../api/devicemanagementabstractcomplexsettinginstance-create.md)|[deviceManagementAbstractComplexSettingInstance](../resources/deviceManagementAbstractComplexSettingInstance.md)|Create a new [deviceManagementAbstractComplexSettingInstance](../resources/devicemanagementabstractcomplexsettinginstance.md) object.|
|[Delete deviceManagementAbstractComplexSettingInstance](../api/devicemanagementabstractcomplexsettinginstance-delete.md)|None|Deletes a [deviceManagementAbstractComplexSettingInstance](../resources/devicemanagementabstractcomplexsettinginstance.md).|
|[Update deviceManagementAbstractComplexSettingInstance](../api/devicemanagementabstractcomplexsettinginstance-update.md)|[deviceManagementAbstractComplexSettingInstance](../resources/deviceManagementAbstractComplexSettingInstance.md)|Update the properties of a [deviceManagementAbstractComplexSettingInstance](../resources/devicemanagementabstractcomplexsettinginstance.md) object.|
|[List value](../api/devicemanagementabstractcomplexsettinginstance-list-value.md)|[deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md) collection|Get the deviceManagementSettingInstances from the value navigation property.|
|[Create value](../api/devicemanagementabstractcomplexsettinginstance-post-value.md)|[deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)|Create value by posting to the value collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|definitionId|String|The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|implementationId|String|The definition ID for the chosen implementation of this complex setting|
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
  "@odata.type": "microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "baseType": "microsoft.graph.deviceManagementSettingInstance",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "implementationId": "String"
}
```

