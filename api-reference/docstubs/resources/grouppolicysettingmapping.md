---
title: "groupPolicySettingMapping resource type"
description: "The Group Policy setting to MDM/Intune mapping."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPolicySettingMapping resource type


Namespace: microsoft.graph

The Group Policy setting to MDM/Intune mapping.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicySettingMapping](../api/grouppolicysettingmapping-get.md)|[groupPolicySettingMapping](../resources/grouppolicysettingmapping.md)|Read the properties and relationships of a [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) object.|
|[Update groupPolicySettingMapping](../api/grouppolicysettingmapping-update.md)|[groupPolicySettingMapping](../resources/grouppolicysettingmapping.md)|Update the properties of a [groupPolicySettingMapping](../resources/grouppolicysettingmapping.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|childIdList|String collection|List of Child Ids of the group policy setting.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|intuneSettingDefinitionId|String|The Intune Setting Definition Id|
|intuneSettingUriList|String collection|The list of Intune Setting URIs this group policy setting maps to|
|isMdmSupported|Boolean|Indicates if the setting is supported by Intune or not|
|mdmCspName|String|The CSP name this group policy setting maps to.|
|mdmMinimumOSVersion|Int32|The minimum OS version this mdm setting supports.|
|mdmSettingUri|String|The MDM CSP URI this group policy setting maps to.|
|mdmSupportedState|mdmSupportedState|Indicates if the setting is supported in Mdm or not. Possible values are: `unknown`, `supported`, `unsupported`, `deprecated`.|
|parentId|String|Parent Id of the group policy setting.|
|settingCategory|String|The category the group policy setting is in.|
|settingDisplayName|String|The display name of this group policy setting.|
|settingDisplayValue|String|The display value of this group policy setting.|
|settingDisplayValueType|String|The display value type of this group policy setting.|
|settingName|String|The name of this group policy setting.|
|settingScope|groupPolicySettingScope|The scope of the setting. Possible values are: `unknown`, `device`, `user`.|
|settingType|groupPolicySettingType|The setting type (security or admx) of the Group Policy. Possible values are: `unknown`, `policy`, `account`, `securityOptions`, `userRightsAssignment`, `auditSetting`, `windowsFirewallSettings`.|
|settingValue|String|The value of this group policy setting.|
|settingValueDisplayUnits|String|The display units of this group policy setting value|
|settingValueType|String|The value type of this group policy setting.|

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

