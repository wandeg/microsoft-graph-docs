---
title: "groupPolicySettingMapping resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicySettingMapping resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicySettingMapping](../api/grouppolicysettingmapping-get.md)|[groupPolicySettingMapping](../resources/grouppolicysettingmapping.md)|Read properties and relationships of the [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) object.|
|[Update groupPolicySettingMapping](../api/grouppolicysettingmapping-update.md)|[groupPolicySettingMapping](../resources/grouppolicysettingmapping.md)|Update the properties of a [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|childIdList|String collection||
|id|String| Inherited from [entity](../resources/entity.md)|
|intuneSettingDefinitionId|String||
|intuneSettingUriList|String collection||
|isMdmSupported|Boolean||
|mdmCspName|String||
|mdmMinimumOSVersion|Int32||
|mdmSettingUri|String||
|mdmSupportedState|Enumeration| Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.|
|parentId|String||
|settingCategory|String||
|settingDisplayName|String||
|settingDisplayValue|String||
|settingDisplayValueType|String||
|settingName|String||
|settingScope|Enumeration| Possible values are: `unknown`, `device`, `user`.|
|settingType|Enumeration| Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.|
|settingValue|String||
|settingValueDisplayUnits|String||
|settingValueType|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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
  "mdmMinimumOSVersion": 1024,
  "settingType": "String",
  "isMdmSupported": true,
  "mdmSupportedState": "String",
  "settingScope": "String",
  "intuneSettingUriList": [
    "String"
  ],
  "intuneSettingDefinitionId": "String"
}
```

