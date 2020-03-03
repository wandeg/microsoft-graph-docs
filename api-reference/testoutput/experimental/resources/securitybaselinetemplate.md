---
title: "securityBaselineTemplate resource type"
description: "The security baseline template of the account"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# securityBaselineTemplate resource type


Namespace: microsoft.graph

The security baseline template of the account


Inherits from [deviceManagementTemplate](../resources/devicemanagementtemplate.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List securityBaselineTemplates](../api/securitybaselinetemplate-list.md)|[securityBaselineTemplate](../resources/securitybaselinetemplate.md) collection|List properties and relationships of the [securityBaselineTemplate](../resources/securitybaselinetemplate.md) objects.|
|[Get securityBaselineTemplate](../api/securitybaselinetemplate-get.md)|[securityBaselineTemplate](../resources/securitybaselinetemplate.md)|Read properties and relationships of the [securityBaselineTemplate](../resources/securitybaselinetemplate.md) object.|
|[Create securityBaselineTemplate](../api/securitybaselinetemplate-create.md)|[securityBaselineTemplate](../resources/securitybaselinetemplate.md)|Create a new [securityBaselineTemplate](../resources/securitybaselinetemplate.md) object.|
|[Delete securityBaselineTemplate](../api/securitybaselinetemplate-delete.md)|None|Deletes a [securityBaselineTemplate](../resources/securitybaselinetemplate.md).|
|[Update securityBaselineTemplate](../api/securitybaselinetemplate-update.md)|[securityBaselineTemplate](../resources/securitybaselinetemplate.md)|Update the properties of a [securityBaselineTemplate](../resources/securitybaselinetemplate.md) object.|
|[createInstance](../api/securitybaselinetemplate-createinstance.md)|[deviceManagementIntent](../resources/devicemanagementintent.md)||
|[compare](../api/securitybaselinetemplate-compare.md)|[deviceManagementSettingComparison](../resources/devicemanagementsettingcomparison.md) collection||
|[List settings](../api/securitybaselinetemplate-list-settings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection|Get the deviceManagementSettingInstances from the settings navigation property.|
|[Add settings](../api/securitybaselinetemplate-post-settings.md)|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md)|Add settings by posting to the settings collection.|
|[List categories](../api/securitybaselinetemplate-list-categories.md)|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) collection|Get the deviceManagementTemplateSettingCategories from the categories navigation property.|
|[Add categories](../api/securitybaselinetemplate-post-categories.md)|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md)|Add categories by posting to the categories collection.|
|[List migratableTo](../api/securitybaselinetemplate-list-migratableto.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md) collection|Get the deviceManagementTemplates from the migratableTo navigation property.|
|[Add migratableTo](../api/securitybaselinetemplate-post-migratableto.md)|[deviceManagementTemplate](../resources/devicemanagementtemplate.md)|Add migratableTo by posting to the migratableTo collection.|
|[Get securityBaselineStateSummary](../api/securitybaselinestatesummary-get.md)|[securityBaselineStateSummary](../resources/securitybaselinestatesummary.md)|Read properties and relationships of the [securityBaselineStateSummary](../resources/securitybaselinestatesummary.md) object.|
|[List deviceStates](../api/securitybaselinetemplate-list-devicestates.md)|[securityBaselineDeviceState](../resources/securitybaselinedevicestate.md) collection|Get the securityBaselineDeviceStates from the deviceStates navigation property.|
|[Add deviceStates](../api/securitybaselinetemplate-post-devicestates.md)|[securityBaselineDeviceState](../resources/securitybaselinedevicestate.md)|Add deviceStates by posting to the deviceStates collection.|
|[List categoryDeviceStateSummaries](../api/securitybaselinetemplate-list-categorydevicestatesummaries.md)|[securityBaselineCategoryStateSummary](../resources/securitybaselinecategorystatesummary.md) collection|Get the securityBaselineCategoryStateSummaries from the categoryDeviceStateSummaries navigation property.|
|[Add categoryDeviceStateSummaries](../api/securitybaselinetemplate-post-categorydevicestatesummaries.md)|[securityBaselineCategoryStateSummary](../resources/securitybaselinecategorystatesummary.md)|Add categoryDeviceStateSummaries by posting to the categoryDeviceStateSummaries collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|The template's description Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md)|
|displayName|String|The template's display name Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|intentCount|Int32|Number of Intents created from this template. Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md)|
|isDeprecated|Boolean|The template is deprecated or not. Intents cannot be created from a deprecated template. Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md)|
|platformType|Enumeration|The template's platform. Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md). Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|publishedDateTime|DateTimeOffset|When the template was published Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md)|
|templateType|Enumeration|The template's type. Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md). Possible values are: `securityBaseline`, `specializedDevices`, `advancedThreatProtectionSecurityBaseline`, `deviceConfiguration`, `custom`, `securityTemplate`, `microsoftEdgeSecurityBaseline`, `microsoftOffice365ProPlusSecurityBaseline`.|
|versionInfo|String|The template's version information Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|categories|[deviceManagementTemplateSettingCategory](../resources/devicemanagementtemplatesettingcategory.md) collection|Collection of setting categories within the template Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md)|
|categoryDeviceStateSummaries|[securityBaselineCategoryStateSummary](../resources/securitybaselinecategorystatesummary.md) collection|The security baseline per category device state summary|
|deviceStates|[securityBaselineDeviceState](../resources/securitybaselinedevicestate.md) collection|The security baseline device states|
|deviceStateSummary|[securityBaselineStateSummary](../resources/securitybaselinestatesummary.md)|The security baseline device state summary|
|migratableTo|[deviceManagementTemplate](../resources/devicemanagementtemplate.md) collection|Collection of templates this template can migrate to Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md)|
|settings|[deviceManagementSettingInstance](../resources/devicemanagementsettinginstance.md) collection|Collection of all settings this template has Inherited from [deviceManagementTemplate](../resources/devicemanagementtemplate.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineTemplate",
  "baseType": "microsoft.graph.deviceManagementTemplate",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
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

