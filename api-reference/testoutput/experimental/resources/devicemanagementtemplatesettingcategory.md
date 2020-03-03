---
title: "deviceManagementTemplateSettingCategory resource type"
description: "Entity representing a template setting category"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementTemplateSettingCategory resource type


Namespace: microsoft.graph

Entity representing a template setting category


Inherits from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List deviceManagementTemplateSettingCategories](../api/devicemanagementtemplatesettingcategory-list.md)|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) collection|List properties and relationships of the [deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) objects.|
|[Get deviceManagementTemplateSettingCategory](../api/devicemanagementtemplatesettingcategory-get.md)|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md)|Read properties and relationships of the [deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) object.|
|[Create deviceManagementTemplateSettingCategory](../api/devicemanagementtemplatesettingcategory-create.md)|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md)|Create a new [deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) object.|
|[Delete deviceManagementTemplateSettingCategory](../api/devicemanagementtemplatesettingcategory-delete.md)|None|Deletes a [deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md).|
|[Update deviceManagementTemplateSettingCategory](../api/devicemanagementtemplatesettingcategory-update.md)|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md)|Update the properties of a [deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) object.|
|[List settingDefinitions](../api/devicemanagementtemplatesettingcategory-list-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection|Get the deviceManagementSettingDefinitions from the settingDefinitions navigation property.|
|[Add settingDefinitions](../api/devicemanagementtemplatesettingcategory-post-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Add settingDefinitions by posting to the settingDefinitions collection.|
|[List recommendedSettings](../api/devicemanagementtemplatesettingcategory-list-recommendedsettings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection|Get the deviceManagementSettingInstances from the recommendedSettings navigation property.|
|[Add recommendedSettings](../api/devicemanagementtemplatesettingcategory-post-recommendedsettings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|Add recommendedSettings by posting to the recommendedSettings collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The category name Inherited from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|recommendedSettings|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection|The settings this category contains|
|settingDefinitions|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection|The setting definitions this category contains Inherited from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTemplateSettingCategory",
  "baseType": "microsoft.graph.deviceManagementSettingCategory",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "id": "String (identifier)",
  "displayName": "String"
}
```

