---
title: "securityBaselineSettingState resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# securityBaselineSettingState resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get securityBaselineSettingState](../api/securitybaselinesettingstate-get.md)|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md)|Read properties and relationships of the [securityBaselineSettingState](../resources/securitybaselinesettingstate.md) object.|
|[Update securityBaselineSettingState](../api/securitybaselinesettingstate-update.md)|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md)|Update the properties of a [securityBaselineSettingState](../resources/securitybaselinesettingstate.md) object.|
|[List settingStates](../api/securitybaselinestate-list-settingstates.md)|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md) collection|Get the securityBaselineSettingStates from the settingStates navigation property.|
|[Add settingStates](../api/securitybaselinestate-post-settingstates.md)|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md)|Add settingStates by posting to the settingStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|settingCategoryId|String||
|settingName|String||
|state|Enumeration| Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.|

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

