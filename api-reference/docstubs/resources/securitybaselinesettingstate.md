---
title: "securityBaselineSettingState resource type"
description: "The security baseline compliance state of a setting for a device"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# securityBaselineSettingState resource type


Namespace: microsoft.graph

The security baseline compliance state of a setting for a device


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get securityBaselineSettingState](../api/securitybaselinesettingstate-get.md)|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md)|Read the properties and relationships of a [securityBaselineSettingState](../resources/securitybaselinesettingstate.md) object.|
|[Update securityBaselineSettingState](../api/securitybaselinesettingstate-update.md)|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md)|Update the properties of a [securityBaselineSettingState](../resources/securitybaselinesettingstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|settingCategoryId|String|The setting category id which this setting belongs to|
|settingName|String|The setting name that is being reported|
|state|securityBaselineComplianceState|The compliance state of the security baseline setting. Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineSettingState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "id": "String (identifier)",
  "settingName": "String",
  "state": "String",
  "settingCategoryId": "String"
}
```

