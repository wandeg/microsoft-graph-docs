---
title: "deviceManagementAbstractComplexSettingDefinition resource type"
description: "Entity representing the defintion for an abstract complex setting"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementAbstractComplexSettingDefinition resource type

Entity representing the defintion for an abstract complex setting


Inherits from [deviceManagementSettingDefinition](../resources/deviceManagementSettingDefinition.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementAbstractComplexSettingDefinitions](../api/devicemanagementabstractcomplexsettingdefinition-list.md)|[deviceManagementAbstractComplexSettingDefinition](../resources/deviceManagementAbstractComplexSettingDefinition.md) collection|List properties and relationships of the [deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md) objects.|
|[Get deviceManagementAbstractComplexSettingDefinition](../api/devicemanagementabstractcomplexsettingdefinition-get.md)|[deviceManagementAbstractComplexSettingDefinition](../resources/deviceManagementAbstractComplexSettingDefinition.md)|Read properties and relationships of the [deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md) object.|
|[Create deviceManagementAbstractComplexSettingDefinition](../api/devicemanagementabstractcomplexsettingdefinition-create.md)|[deviceManagementAbstractComplexSettingDefinition](../resources/deviceManagementAbstractComplexSettingDefinition.md)|Create a new [deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md) object.|
|[Delete deviceManagementAbstractComplexSettingDefinition](../api/devicemanagementabstractcomplexsettingdefinition-delete.md)|None|Deletes a [deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md).|
|[Update deviceManagementAbstractComplexSettingDefinition](../api/devicemanagementabstractcomplexsettingdefinition-update.md)|[deviceManagementAbstractComplexSettingDefinition](../resources/deviceManagementAbstractComplexSettingDefinition.md)|Update the properties of a [deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|constraints|[deviceManagementConstraint](../resources/deviceManagementConstraint.md) collection|Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/deviceManagementSettingDefinition.md)|
|dependencies|[deviceManagementSettingDependency](../resources/deviceManagementSettingDependency.md) collection|Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/deviceManagementSettingDefinition.md)|
|description|String|The setting's description Inherited from [deviceManagementSettingDefinition](../resources/deviceManagementSettingDefinition.md)|
|displayName|String|The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/deviceManagementSettingDefinition.md)|
|documentationUrl|String|Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/deviceManagementSettingDefinition.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|implementations|String collection|List of definition IDs for all possible implementations of this abstract complex setting|
|isTopLevel|Boolean|If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/deviceManagementSettingDefinition.md)|
|keywords|String collection|Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/deviceManagementSettingDefinition.md)|
|valueType|Enumeration|The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/deviceManagementSettingDefinition.md). Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
  "baseType": "microsoft.graph.deviceManagementSettingDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
  "id": "String (identifier)",
  "valueType": "String",
  "displayName": "String",
  "isTopLevel": true,
  "description": "String",
  "documentationUrl": "String",
  "keywords": [
    "String"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingXmlConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency"
    }
  ],
  "implementations": [
    "String"
  ]
}
```

