---
title: "deviceManagementTemplateSettingCategory resource type"
description: "Entity representing a template setting category"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementTemplateSettingCategory resource type


Namespace: microsoft.graph

Entity representing a template setting category


Inherits from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementTemplateSettingCategory](../api/devicemanagementtemplatesettingcategory-get.md)|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md)|Read the properties and relationships of a [deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) object.|
|[Update deviceManagementTemplateSettingCategory](../api/devicemanagementtemplatesettingcategory-update.md)|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md)|Update the properties of a [deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) object.|
|[List settingDefinitions](../api/devicemanagementtemplatesettingcategory-list-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection|Get the deviceManagementSettingDefinitions from the settingDefinitions navigation property.|
|[Create settingDefinitions](../api/devicemanagementtemplatesettingcategory-post-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Create a new settingDefinitions object.|
|[Delete settingDefinitions](../api/devicemanagementtemplatesettingcategory-delete-settingdefinitions.md)|None|Delete a [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) object.|
|[Update settingDefinitions](../api/devicemanagementtemplatesettingcategory-update-settingdefinitions.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Update the properties of a settingDefinitions object.|
|[Get deviceManagementSettingDefinition](../api/devicemanagementsettingdefinition-get.md)|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|Read the properties and relationships of a [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) object.|
|[List recommendedSettings](../api/devicemanagementtemplatesettingcategory-list-recommendedsettings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection|Get the deviceManagementSettingInstances from the recommendedSettings navigation property.|
|[Create recommendedSettings](../api/devicemanagementtemplatesettingcategory-post-recommendedsettings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|Create a new recommendedSettings object.|
|[Delete recommendedSettings](../api/devicemanagementtemplatesettingcategory-delete-recommendedsettings.md)|None|Delete a [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) object.|
|[Update recommendedSettings](../api/devicemanagementtemplatesettingcategory-update-recommendedsettings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|Update the properties of a recommendedSettings object.|
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
|recommendedSettings|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection|The settings this category contains|
|settingDefinitions|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection|The setting definitions this category contains Inherited from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|

## JSON representation
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
  "displayName": "String",
  "hasRequiredSetting": true
}
```

