---
title: "deviceManagementSettingDefinition resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementSettingDefinition resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementSettingDefinition](../api/devicemanagementsettingdefinition-get.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Read properties and relationships of the [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) object.|
|[Update deviceManagementSettingDefinition](../api/devicemanagementsettingdefinition-update.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Update the properties of a [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) object.|
|[List settingDefinitions](../api/devicemanagementsettingcategory-list-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection|Get the deviceManagementSettingDefinitions from the settingDefinitions navigation property.|
|[Add settingDefinitions](../api/devicemanagementsettingcategory-post-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Add settingDefinitions by posting to the settingDefinitions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|constraints|[deviceManagementConstraint](../resources/devicemanagementconstraint.md) collection||
|dependencies|[deviceManagementSettingDependency](../resources/devicemanagementsettingdependency.md) collection||
|description|String||
|displayName|String||
|documentationUrl|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isTopLevel|Boolean||
|keywords|String collection||
|placeholderText|String||
|valueType|Enumeration| Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.|

## Relationships
None

## JSON representation
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
  "placeholderText": "String",
  "documentationUrl": "String",
  "keywords": [
    "String"
  ],
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingAppConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency"
    }
  ]
}
```

