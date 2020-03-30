---
title: "deviceManagementSettingCategory resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementSettingCategory resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementSettingCategory](../api/devicemanagementsettingcategory-get.md)|[deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|Read properties and relationships of the [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) object.|
|[Update deviceManagementSettingCategory](../api/devicemanagementsettingcategory-update.md)|[deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|Update the properties of a [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) object.|
|[List settingDefinitions](../api/devicemanagementsettingcategory-list-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection|Get the deviceManagementSettingDefinitions from the settingDefinitions navigation property.|
|[Add settingDefinitions](../api/devicemanagementsettingcategory-post-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Add settingDefinitions by posting to the settingDefinitions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|hasRequiredSetting|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|settingDefinitions|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingCategory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "hasRequiredSetting": true
}
```

