---
title: "deviceManagementTemplate resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementTemplate resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[createInstance](../api/devicemanagementtemplate-createinstance.md)|[deviceManagementIntent](../resources/devicemanagementintent.md)|**TODO: Add Description**|
|[compare](../api/devicemanagementtemplate-compare.md)|[deviceManagementSettingComparison](../resources/devicemanagementsettingcomparison.md) collection|**TODO: Add Description**|
|[List settings](../api/devicemanagementtemplate-list-settings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection|Get the deviceManagementSettingInstances from the settings navigation property.|
|[Create settings](../api/devicemanagementtemplate-post-settings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|Create a new settings object.|
|[Delete settings](../api/devicemanagementtemplate-delete-settings.md)|None|Delete a [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) object.|
|[Update settings](../api/devicemanagementtemplate-update-settings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|Update the properties of a settings object.|
|[Get deviceManagementSettingInstance](../api/devicemanagementsettinginstance-get.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|Read the properties and relationships of a [deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) object.|
|[List categories](../api/devicemanagementtemplate-list-categories.md)|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) collection|Get the deviceManagementTemplateSettingCategories from the categories navigation property.|
|[Create categories](../api/devicemanagementtemplate-post-categories.md)|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md)|Create a new categories object.|
|[Delete categories](../api/devicemanagementtemplate-delete-categories.md)|None|Delete a [deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) object.|
|[Update categories](../api/devicemanagementtemplate-update-categories.md)|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md)|Update the properties of a categories object.|
|[Get deviceManagementTemplateSettingCategory](../api/devicemanagementtemplatesettingcategory-get.md)|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md)|Read the properties and relationships of a [deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) object.|
|[List migratableTo](../api/devicemanagementtemplate-list-migratableto.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md) collection|Get the deviceManagementTemplates from the migratableTo navigation property.|
|[Create migratableTo](../api/devicemanagementtemplate-post-migratableto.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md)|Create a new migratableTo object.|
|[Delete migratableTo](../api/devicemanagementtemplate-delete-migratableto.md)|None|Delete a [deviceManagementTemplate](../resources/devicemanagementtemplate.md) object.|
|[Update migratableTo](../api/devicemanagementtemplate-update-migratableto.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md)|Update the properties of a migratableTo object.|
|[Get deviceManagementTemplate](../api/devicemanagementtemplate-get.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md)|Read the properties and relationships of a [deviceManagementTemplate](../resources/devicemanagementtemplate.md) object.|
|[List migratableTo](../api/devicemanagementtemplate-list-migratableto.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md) collection|Get the deviceManagementTemplates from the migratableTo navigation property.|
|[Create migratableTo](../api/devicemanagementtemplate-post-migratableto.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md)|Create a new migratableTo object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|intentCount|Int32|**TODO: Add Description**|
|isDeprecated|Boolean|**TODO: Add Description**|
|platformType|policyPlatformType|**TODO: Add Description**. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.|
|publishedDateTime|DateTimeOffset|**TODO: Add Description**|
|templateType|deviceManagementTemplateType|**TODO: Add Description**. Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`, `deviceCompliance`.|
|versionInfo|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|categories|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) collection|**TODO: Add Description**|
|migratableTo|[deviceManagementTemplate](../resources/devicemanagementtemplate.md) collection|**TODO: Add Description**|
|settings|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTemplate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "versionInfo": "String",
  "isDeprecated": "Boolean",
  "intentCount": "Integer",
  "templateType": "String",
  "platformType": "String",
  "publishedDateTime": "String (timestamp)"
}
```

