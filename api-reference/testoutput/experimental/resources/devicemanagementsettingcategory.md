---
title: "deviceManagementSettingCategory resource type"
description: "Entity representing a setting category"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementSettingCategory resource type


Namespace: microsoft.graph

Entity representing a setting category


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementSettingCategories](../api/devicemanagementsettingcategory-list.md)|[deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) collection|List properties and relationships of the [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) objects.|
|[Get deviceManagementSettingCategory](../api/devicemanagementsettingcategory-get.md)|[deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|Read properties and relationships of the [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) object.|
|[Create deviceManagementSettingCategory](../api/devicemanagementsettingcategory-create.md)|[deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|Create a new [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) object.|
|[Delete deviceManagementSettingCategory](../api/devicemanagementsettingcategory-delete.md)|None|Deletes a [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md).|
|[Update deviceManagementSettingCategory](../api/devicemanagementsettingcategory-update.md)|[deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|Update the properties of a [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) object.|
|[List settingDefinitions](../api/devicemanagementsettingcategory-list-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection|Get the deviceManagementSettingDefinitions from the settingDefinitions navigation property.|
|[Add settingDefinitions](../api/devicemanagementsettingcategory-post-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Add settingDefinitions by posting to the settingDefinitions collection.|
|[List categories](../api/intune-devices-devicemanagement-list-categories.md)|[deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md) collection|Get the deviceManagementSettingCategories from the categories navigation property.|
|[Add categories](../api/intune-devices-devicemanagement-post-categories.md)|[deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|Add categories by posting to the categories collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The category name|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|settingDefinitions|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection|The setting definitions this category contains|

## JSON Representation
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
  "displayName": "String"
}
```

