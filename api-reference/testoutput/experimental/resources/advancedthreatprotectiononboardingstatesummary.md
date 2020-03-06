---
title: "advancedThreatProtectionOnboardingStateSummary resource type"
description: "Windows defender advanced threat protection onboarding state summary across the account."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# advancedThreatProtectionOnboardingStateSummary resource type


Namespace: microsoft.graph

Windows defender advanced threat protection onboarding state summary across the account.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get advancedThreatProtectionOnboardingStateSummary](../api/advancedthreatprotectiononboardingstatesummary-get.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md)|Read properties and relationships of the [advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md) object.|
|[Update advancedThreatProtectionOnboardingStateSummary](../api/advancedthreatprotectiononboardingstatesummary-update.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md)|Update the properties of a [advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md) object.|
|[List advancedThreatProtectionOnboardingDeviceSettingStates](../api/advancedthreatprotectiononboardingstatesummary-list-advancedthreatprotectiononboardingdevicesettingstates.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md) collection|Get the advancedThreatProtectionOnboardingDeviceSettingStates from the advancedThreatProtectionOnboardingDeviceSettingStates navigation property.|
|[Add advancedThreatProtectionOnboardingDeviceSettingStates](../api/advancedthreatprotectiononboardingstatesummary-post-advancedthreatprotectiononboardingdevicesettingstates.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md)|Add advancedThreatProtectionOnboardingDeviceSettingStates by posting to the advancedThreatProtectionOnboardingDeviceSettingStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantDeviceCount|Int32|Number of compliant devices|
|conflictDeviceCount|Int32|Number of conflict devices|
|errorDeviceCount|Int32|Number of error devices|
|id|String| Inherited from [entity](../resources/entity.md)|
|nonCompliantDeviceCount|Int32|Number of NonCompliant devices|
|notApplicableDeviceCount|Int32|Number of not applicable devices|
|notAssignedDeviceCount|Int32|Number of not assigned devices|
|remediatedDeviceCount|Int32|Number of remediated devices|
|unknownDeviceCount|Int32|Number of unknown devices|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|advancedThreatProtectionOnboardingDeviceSettingStates|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingStateSummary",
  "id": "String (identifier)",
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notAssignedDeviceCount": 1024
}
```

