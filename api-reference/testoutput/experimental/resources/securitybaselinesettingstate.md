---
title: "securityBaselineSettingState resource type"
description: "The security baseline compliance state of a setting for a device"
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# securityBaselineSettingState resource type

The security baseline compliance state of a setting for a device


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get securityBaselineSettingState](../api/securitybaselinesettingstate-get.md)|[securityBaselineSettingState](../resources/securityBaselineSettingState.md)|Read properties and relationships of the [securityBaselineSettingState](../resources/securitybaselinesettingstate.md) object.|
|[Delete securityBaselineSettingState](../api/securitybaselinesettingstate-delete.md)|None|Deletes a [securityBaselineSettingState](../resources/securitybaselinesettingstate.md).|
|[Update securityBaselineSettingState](../api/securitybaselinesettingstate-update.md)|[securityBaselineSettingState](../resources/securityBaselineSettingState.md)|Update the properties of a [securityBaselineSettingState](../resources/securitybaselinesettingstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|settingCategoryId|String|The setting category id which this setting belongs to|
|settingName|String|The setting name that is being reported|
|state|Enumeration|The compliance state of the security baseline setting. Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.|

## Relationships
None

## JSON Representation
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

