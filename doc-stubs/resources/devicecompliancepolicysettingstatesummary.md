---
title: "deviceCompliancePolicySettingStateSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceCompliancePolicySettingStateSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List deviceComplianceSettingStates](../api/devicecompliancepolicysettingstatesummary-list-devicecompliancesettingstates.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) collection|Get the deviceComplianceSettingStates from the deviceComplianceSettingStates navigation property.|
|[Create deviceComplianceSettingStates](../api/devicecompliancepolicysettingstatesummary-post-devicecompliancesettingstates.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md)|Create a new deviceComplianceSettingStates object.|
|[Delete deviceComplianceSettingStates](../api/devicecompliancepolicysettingstatesummary-delete-devicecompliancesettingstates.md)|None|Delete a [deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) object.|
|[Update deviceComplianceSettingStates](../api/devicecompliancepolicysettingstatesummary-update-devicecompliancesettingstates.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md)|Update the properties of a deviceComplianceSettingStates object.|
|[Get deviceComplianceSettingState](../api/devicecompliancesettingstate-get.md)|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md)|Read the properties and relationships of a [deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantDeviceCount|Int32|**TODO: Add Description**|
|conflictDeviceCount|Int32|**TODO: Add Description**|
|errorDeviceCount|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|nonCompliantDeviceCount|Int32|**TODO: Add Description**|
|notApplicableDeviceCount|Int32|**TODO: Add Description**|
|platformType|policyPlatformType|**TODO: Add Description**. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.|
|remediatedDeviceCount|Int32|**TODO: Add Description**|
|setting|String|**TODO: Add Description**|
|settingName|String|**TODO: Add Description**|
|unknownDeviceCount|Int32|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deviceComplianceSettingStates|[deviceComplianceSettingState](../resources/devicecompliancesettingstate.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "unknownDeviceCount": "Integer",
  "notApplicableDeviceCount": "Integer",
  "compliantDeviceCount": "Integer",
  "remediatedDeviceCount": "Integer",
  "nonCompliantDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "conflictDeviceCount": "Integer"
}
```

