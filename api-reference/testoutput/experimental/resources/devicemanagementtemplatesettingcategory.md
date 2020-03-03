---
title: "deviceManagementTemplateSettingCategory resource type"
description: "Entity representing a template setting category"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceManagementTemplateSettingCategory resource type

Entity representing a template setting category


Inherits from [deviceManagementSettingCategory](../resources/deviceManagementSettingCategory.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementTemplateSettingCategory](../api/devicemanagementtemplatesettingcategory-get.md)|[deviceManagementTemplateSettingCategory](../resources/deviceManagementTemplateSettingCategory.md)|Read properties and relationships of the [deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) object.|
|[Delete deviceManagementTemplateSettingCategory](../api/devicemanagementtemplatesettingcategory-delete.md)|None|Deletes a [deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md).|
|[Update deviceManagementTemplateSettingCategory](../api/devicemanagementtemplatesettingcategory-update.md)|[deviceManagementTemplateSettingCategory](../resources/deviceManagementTemplateSettingCategory.md)|Update the properties of a [deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) object.|
|[List settingDefinitions](../api/devicemanagementtemplatesettingcategory-list-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/deviceManagementSettingDefinition.md) collection|Get the deviceManagementSettingDefinitions from the settingDefinitions navigation property.|
|[Add settingDefinitions](../api/devicemanagementtemplatesettingcategory-post-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/deviceManagementSettingDefinition.md)|Add settingDefinitions by posting to the settingDefinitions collection.|
|[List recommendedSettings](../api/devicemanagementtemplatesettingcategory-list-recommendedsettings.md)|[deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md) collection|Get the deviceManagementSettingInstances from the recommendedSettings navigation property.|
|[Add recommendedSettings](../api/devicemanagementtemplatesettingcategory-post-recommendedsettings.md)|[deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md)|Add recommendedSettings by posting to the recommendedSettings collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The category name Inherited from [deviceManagementSettingCategory](../resources/deviceManagementSettingCategory.md)|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|recommendedSettings|[deviceManagementSettingInstance](../resources/deviceManagementSettingInstance.md) collection|The settings this category contains|
|settingDefinitions|[deviceManagementSettingDefinition](../resources/deviceManagementSettingDefinition.md) collection|The setting definitions this category contains Inherited from [deviceManagementSettingCategory](../resources/deviceManagementSettingCategory.md)|

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

