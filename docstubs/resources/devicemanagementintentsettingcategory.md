---
title: "deviceManagementIntentSettingCategory resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementIntentSettingCategory resource type


Namespace: microsoft.graph




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

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String| Inherited from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|
|hasRequiredSetting|Boolean| Inherited from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|settingDefinitions|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection| Inherited from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|
|settings|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection||

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
  "displayName": "String",
  "hasRequiredSetting": true
}
```

