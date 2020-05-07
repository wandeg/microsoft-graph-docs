---
title: "groupPolicySettingMapping resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPolicySettingMapping resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|childIdList|String collection|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|intuneSettingDefinitionId|String|**TODO: Add Description**|
|intuneSettingUriList|String collection|**TODO: Add Description**|
|isMdmSupported|Boolean|**TODO: Add Description**|
|mdmCspName|String|**TODO: Add Description**|
|mdmMinimumOSVersion|Int32|**TODO: Add Description**|
|mdmSettingUri|String|**TODO: Add Description**|
|mdmSupportedState|mdmSupportedState|**TODO: Add Description**. Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.|
|parentId|String|**TODO: Add Description**|
|settingCategory|String|**TODO: Add Description**|
|settingDisplayName|String|**TODO: Add Description**|
|settingDisplayValue|String|**TODO: Add Description**|
|settingDisplayValueType|String|**TODO: Add Description**|
|settingName|String|**TODO: Add Description**|
|settingScope|groupPolicySettingScope|**TODO: Add Description**. Possible values are: `unknown`, `device`, `user`.|
|settingType|groupPolicySettingType|**TODO: Add Description**. Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.|
|settingValue|String|**TODO: Add Description**|
|settingValueDisplayUnits|String|**TODO: Add Description**|
|settingValueType|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicySettingMapping",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicySettingMapping",
  "id": "String (identifier)",
  "parentId": "String",
  "childIdList": [
    "String"
  ],
  "settingName": "String",
  "settingValue": "String",
  "settingValueType": "String",
  "settingDisplayName": "String",
  "settingDisplayValue": "String",
  "settingDisplayValueType": "String",
  "settingValueDisplayUnits": "String",
  "settingCategory": "String",
  "mdmCspName": "String",
  "mdmSettingUri": "String",
  "mdmMinimumOSVersion": "Integer",
  "settingType": "String",
  "isMdmSupported": "Boolean",
  "mdmSupportedState": "String",
  "settingScope": "String",
  "intuneSettingUriList": [
    "String"
  ],
  "intuneSettingDefinitionId": "String"
}
```

