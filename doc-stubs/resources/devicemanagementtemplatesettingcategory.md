---
title: "deviceManagementTemplateSettingCategory resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementTemplateSettingCategory resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
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
|[List categories](../api/devicemanagementtemplate-list-categories.md)|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) collection|Get the deviceManagementTemplateSettingCategories from the categories navigation property.|
|[Create categories](../api/devicemanagementtemplate-post-categories.md)|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md)|Create a new categories object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description** Inherited from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|
|hasRequiredSetting|Boolean|**TODO: Add Description** Inherited from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|recommendedSettings|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection|**TODO: Add Description**|
|settingDefinitions|[deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md) collection|**TODO: Add Description** Inherited from [deviceManagementSettingCategory](../resources/devicemanagementsettingcategory.md)|

## JSON representation
The following is a JSON representation of the resource.
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
  "hasRequiredSetting": "Boolean"
}
```

