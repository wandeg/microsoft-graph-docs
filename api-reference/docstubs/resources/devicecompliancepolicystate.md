---
title: "deviceCompliancePolicyState resource type"
description: "Device Compliance Policy State for a given device."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceCompliancePolicyState resource type


Namespace: microsoft.graph

Device Compliance Policy State for a given device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceCompliancePolicyState](../api/devicecompliancepolicystate-get.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md)|Read the properties and relationships of a [deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) object.|
|[Update deviceCompliancePolicyState](../api/devicecompliancepolicystate-update.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md)|Update the properties of a [deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) object.|
|[List deviceCompliancePolicyStates](../api/manageddevice-list-devicecompliancepolicystates.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) collection|Get the deviceCompliancePolicyStates from the deviceCompliancePolicyStates navigation property.|
|[Create deviceCompliancePolicyStates](../api/manageddevice-post-devicecompliancepolicystates.md)|[deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md)|Create a new deviceCompliancePolicyStates object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The name of the policy for this policyBase|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|platformType|policyPlatformType|Platform type that the policy applies to. Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|settingCount|Int32|Count of how many setting a policy holds|
|settingStates|[deviceCompliancePolicySettingState](../resources/devicecompliancepolicysettingstate.md) collection|**TODO: Add Description**|
|state|complianceStatus|The compliance state of the policy. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|version|Int32|The version of the policy|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
  "id": "String (identifier)",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState"
    }
  ],
  "displayName": "String",
  "version": 1024,
  "platformType": "String",
  "state": "String",
  "settingCount": 1024
}
```

