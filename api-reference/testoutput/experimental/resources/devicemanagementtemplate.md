---
title: "deviceManagementTemplate resource type"
description: "Entity that represents a defined collection of device settings"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementTemplate resource type


Namespace: microsoft.graph

Entity that represents a defined collection of device settings


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementTemplate](../api/devicemanagementtemplate-get.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md)|Read properties and relationships of the [deviceManagementTemplate](../resources/devicemanagementtemplate.md) object.|
|[Update deviceManagementTemplate](../api/devicemanagementtemplate-update.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md)|Update the properties of a [deviceManagementTemplate](../resources/devicemanagementtemplate.md) object.|
|[createInstance](../api/devicemanagementtemplate-createinstance.md)|[deviceManagementIntent](../resources/devicemanagementintent.md)||
|[compare](../api/devicemanagementtemplate-compare.md)|[deviceManagementSettingComparison](../resources/devicemanagementsettingcomparison.md) collection||
|[List settings](../api/devicemanagementtemplate-list-settings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection|Get the deviceManagementSettingInstances from the settings navigation property.|
|[Add settings](../api/devicemanagementtemplate-post-settings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|Add settings by posting to the settings collection.|
|[List categories](../api/devicemanagementtemplate-list-categories.md)|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) collection|Get the deviceManagementTemplateSettingCategories from the categories navigation property.|
|[Add categories](../api/devicemanagementtemplate-post-categories.md)|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md)|Add categories by posting to the categories collection.|
|[List migratableTo](../api/devicemanagementtemplate-list-migratableto.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md) collection|Get the deviceManagementTemplates from the migratableTo navigation property.|
|[Add migratableTo](../api/devicemanagementtemplate-post-migratableto.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md)|Add migratableTo by posting to the migratableTo collection.|
|[List migratableTo](../api/devicemanagementtemplate-list-migratableto.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md) collection|Get the deviceManagementTemplates from the migratableTo navigation property.|
|[Add migratableTo](../api/devicemanagementtemplate-post-migratableto.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md)|Add migratableTo by posting to the migratableTo collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|The template's description|
|displayName|String|The template's display name|
|id|String| Inherited from [entity](../resources/entity.md)|
|intentCount|Int32|Number of Intents created from this template.|
|isDeprecated|Boolean|The template is deprecated or not. Intents cannot be created from a deprecated template.|
|platformType|Enumeration|The template's platform. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|publishedDateTime|DateTimeOffset|When the template was published|
|templateType|Enumeration|The template's type. Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`.|
|versionInfo|String|The template's version information|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|categories|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) collection|Collection of setting categories within the template|
|migratableTo|[deviceManagementTemplate](../resources/devicemanagementtemplate.md) collection|Collection of templates this template can migrate to|
|settings|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection|Collection of all settings this template has|

## JSON representation
Here is a JSON representation of the resource.
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
  "isDeprecated": true,
  "intentCount": 1024,
  "templateType": "String",
  "platformType": "String",
  "publishedDateTime": "String (timestamp)"
}
```

