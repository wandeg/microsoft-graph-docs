---
title: "deviceManagementIntentSettingCategory resource type"
description: "Entity representing an intent setting category"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementIntentSettingCategory resource type


Namespace: microsoft.graph

Entity representing an intent setting category


Inherits from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementIntentSettingCategory](../api/devicemanagementintentsettingcategory-get.md)|[deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md)|Read properties and relationships of the [deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md) object.|
|[Update deviceManagementIntentSettingCategory](../api/devicemanagementintentsettingcategory-update.md)|[deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md)|Update the properties of a [deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md) object.|
|[List settingDefinitions](../api/devicemanagementintentsettingcategory-list-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection|Get the deviceManagementSettingDefinitions from the settingDefinitions navigation property.|
|[Add settingDefinitions](../api/devicemanagementintentsettingcategory-post-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Add settingDefinitions by posting to the settingDefinitions collection.|
|[List settings](../api/devicemanagementintentsettingcategory-list-settings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection|Get the deviceManagementSettingInstances from the settings navigation property.|
|[Add settings](../api/devicemanagementintentsettingcategory-post-settings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|Add settings by posting to the settings collection.|
|[List categories](../api/devicemanagementintent-list-categories.md)|[deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md) collection|Get the deviceManagementIntentSettingCategories from the categories navigation property.|
|[Add categories](../api/devicemanagementintent-post-categories.md)|[deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md)|Add categories by posting to the categories collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The category name Inherited from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|settingDefinitions|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection|The setting definitions this category contains Inherited from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|
|settings|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection|The settings this category contains|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentSettingCategory",
  "baseType": "microsoft.graph.deviceManagementSettingCategory",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentSettingCategory",
  "id": "String (identifier)",
  "displayName": "String"
}
```

