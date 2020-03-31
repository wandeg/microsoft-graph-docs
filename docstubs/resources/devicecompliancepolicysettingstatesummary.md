---
title: "deviceCompliancePolicySettingStateSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceCompliancePolicySettingStateSummary resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceCompliancePolicySettingStateSummary](../api/devicecompliancepolicysettingstatesummary-get.md)|[deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md)|Read properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) object.|
|[Update deviceCompliancePolicySettingStateSummary](../api/devicecompliancepolicysettingstatesummary-update.md)|[deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md)|Update the properties of a [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) object.|
|[List deviceComplianceSettingStates](../api/devicecompliancepolicysettingstatesummary-list-devicecompliancesettingstates.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) collection|Get the deviceComplianceSettingStates from the deviceComplianceSettingStates navigation property.|
|[Add deviceComplianceSettingStates](../api/devicecompliancepolicysettingstatesummary-post-devicecompliancesettingstates.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md)|Add deviceComplianceSettingStates by posting to the deviceComplianceSettingStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantDeviceCount|Int32||
|conflictDeviceCount|Int32||
|errorDeviceCount|Int32||
|id|String| Inherited from [entity](../resources/entity.md)|
|nonCompliantDeviceCount|Int32||
|notApplicableDeviceCount|Int32||
|platformType|Enumeration| Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|remediatedDeviceCount|Int32||
|setting|String||
|settingName|String||
|unknownDeviceCount|Int32||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deviceComplianceSettingStates|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "String (identifier)",
  "setting": "String",
  "settingName": "String",
  "platformType": "String",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```

