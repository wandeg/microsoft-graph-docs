---
title: "deviceManagementSettingDefinition resource type"
description: "Entity representing the defintion for a given setting"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementSettingDefinition resource type


Namespace: microsoft.graph

Entity representing the defintion for a given setting


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementSettingDefinitions](../api/devicemanagementsettingdefinition-list.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection|List properties and relationships of the [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) objects.|
|[Get deviceManagementSettingDefinition](../api/devicemanagementsettingdefinition-get.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Read properties and relationships of the [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) object.|
|[Create deviceManagementSettingDefinition](../api/devicemanagementsettingdefinition-create.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Create a new [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) object.|
|[Delete deviceManagementSettingDefinition](../api/devicemanagementsettingdefinition-delete.md)|None|Deletes a [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md).|
|[Update deviceManagementSettingDefinition](../api/devicemanagementsettingdefinition-update.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Update the properties of a [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|constraints|[deviceManagementConstraint](../resources/devicemanagementconstraint.md) collection|Collection of constraints for the setting value|
|dependencies|[deviceManagementSettingDependency](../resources/devicemanagementsettingdependency.md) collection|Collection of dependencies on other settings|
|description|String|The setting's description|
|displayName|String|The setting's display name|
|documentationUrl|String|Url to setting documentation|
|id|String| Inherited from [entity](../resources/entity.md)|
|isTopLevel|Boolean|If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting|
|keywords|String collection|Keywords associated with the setting|
|valueType|Enumeration|The data type of the value. Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingDefinition",
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
  ]
}
```

