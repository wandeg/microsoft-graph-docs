---
title: "deviceManagementComplexSettingDefinition resource type"
description: "Entity representing the defintion for a complex setting"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementComplexSettingDefinition resource type


Namespace: microsoft.graph

Entity representing the defintion for a complex setting


Inherits from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementComplexSettingDefinitions](../api/devicemanagementcomplexsettingdefinition-list.md)|[deviceManagementComplexSettingDefinition](../resources/devicemanagementcomplexsettingdefinition.md) collection|List properties and relationships of the [deviceManagementComplexSettingDefinition](../resources/devicemanagementcomplexsettingdefinition.md) objects.|
|[Get deviceManagementComplexSettingDefinition](../api/devicemanagementcomplexsettingdefinition-get.md)|[deviceManagementComplexSettingDefinition](../resources/devicemanagementcomplexsettingdefinition.md)|Read properties and relationships of the [deviceManagementComplexSettingDefinition](../resources/devicemanagementcomplexsettingdefinition.md) object.|
|[Create deviceManagementComplexSettingDefinition](../api/devicemanagementcomplexsettingdefinition-create.md)|[deviceManagementComplexSettingDefinition](../resources/devicemanagementcomplexsettingdefinition.md)|Create a new [deviceManagementComplexSettingDefinition](../resources/devicemanagementcomplexsettingdefinition.md) object.|
|[Delete deviceManagementComplexSettingDefinition](../api/devicemanagementcomplexsettingdefinition-delete.md)|None|Deletes a [deviceManagementComplexSettingDefinition](../resources/devicemanagementcomplexsettingdefinition.md).|
|[Update deviceManagementComplexSettingDefinition](../api/devicemanagementcomplexsettingdefinition-update.md)|[deviceManagementComplexSettingDefinition](../resources/devicemanagementcomplexsettingdefinition.md)|Update the properties of a [deviceManagementComplexSettingDefinition](../resources/devicemanagementcomplexsettingdefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|constraints|[deviceManagementConstraint](../resources/devicemanagementconstraint.md) collection|Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|dependencies|[deviceManagementSettingDependency](../resources/devicemanagementsettingdependency.md) collection|Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|description|String|The setting's description Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|displayName|String|The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|documentationUrl|String|Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isTopLevel|Boolean|If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|keywords|String collection|Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|propertyDefinitionIds|String collection|The definitions of each property of the complex setting|
|valueType|Enumeration|The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md). Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementComplexSettingDefinition",
  "baseType": "microsoft.graph.deviceManagementSettingDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingDefinition",
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
  "propertyDefinitionIds": [
    "String"
  ]
}
```

