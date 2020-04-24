---
title: "deviceManagementIntentSettingCategory resource type"
description: "Entity representing an intent setting category"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementIntentSettingCategory resource type


Namespace: microsoft.graph

Entity representing an intent setting category


Inherits from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementIntentSettingCategory](../api/devicemanagementintentsettingcategory-get.md)|[deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md)|Read the properties and relationships of a [deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md) object.|
|[Update deviceManagementIntentSettingCategory](../api/devicemanagementintentsettingcategory-update.md)|[deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md)|Update the properties of a [deviceManagementIntentSettingCategory](../resources/devicemanagementintentsettingcategory.md) object.|
|[List settingDefinitions](../api/devicemanagementintentsettingcategory-list-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection|Get the deviceManagementSettingDefinitions from the settingDefinitions navigation property.|
|[Create settingDefinitions](../api/devicemanagementintentsettingcategory-post-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Create a new settingDefinitions object.|
|[Delete settingDefinitions](../api/devicemanagementintentsettingcategory-delete-settingdefinitions.md)|None|Delete a [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) object.|
|[Update settingDefinitions](../api/devicemanagementintentsettingcategory-update-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Update the properties of a settingDefinitions object.|
|[Get deviceManagementSettingDefinition](../api/devicemanagementsettingdefinition-get.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Read the properties and relationships of a [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) object.|
|[List settings](../api/devicemanagementintentsettingcategory-list-settings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection|Get the deviceManagementSettingInstances from the settings navigation property.|
|[Create settings](../api/devicemanagementintentsettingcategory-post-settings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|Create a new settings object.|
|[Delete settings](../api/devicemanagementintentsettingcategory-delete-settings.md)|None|Delete a [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) object.|
|[Update settings](../api/devicemanagementintentsettingcategory-update-settings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|Update the properties of a settings object.|
|[Get deviceManagementSettingInstance](../api/devicemanagementsettinginstance-get.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|Read the properties and relationships of a [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The category name Inherited from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|
|hasRequiredSetting|Boolean|The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

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
  "displayName": "String",
  "hasRequiredSetting": true
}
```

