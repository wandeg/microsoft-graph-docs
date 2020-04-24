---
title: "advancedThreatProtectionOnboardingStateSummary resource type"
description: "Windows defender advanced threat protection onboarding state summary across the account."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# advancedThreatProtectionOnboardingStateSummary resource type


Namespace: microsoft.graph

Windows defender advanced threat protection onboarding state summary across the account.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get advancedThreatProtectionOnboardingStateSummary](../api/advancedthreatprotectiononboardingstatesummary-get.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md)|Read the properties and relationships of an [advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md) object.|
|[Update advancedThreatProtectionOnboardingStateSummary](../api/advancedthreatprotectiononboardingstatesummary-update.md)|[advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md)|Update the properties of an [advancedThreatProtectionOnboardingStateSummary](../resources/advancedthreatprotectiononboardingstatesummary.md) object.|
|[List advancedThreatProtectionOnboardingDeviceSettingStates](../api/advancedthreatprotectiononboardingstatesummary-list-advancedthreatprotectiononboardingdevicesettingstates.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md) collection|Get the advancedThreatProtectionOnboardingDeviceSettingStates from the advancedThreatProtectionOnboardingDeviceSettingStates navigation property.|
|[Create advancedThreatProtectionOnboardingDeviceSettingStates](../api/advancedthreatprotectiononboardingstatesummary-post-advancedthreatprotectiononboardingdevicesettingstates.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md)|Create a new advancedThreatProtectionOnboardingDeviceSettingStates object.|
|[Delete advancedThreatProtectionOnboardingDeviceSettingStates](../api/advancedthreatprotectiononboardingstatesummary-delete-advancedthreatprotectiononboardingdevicesettingstates.md)|None|Delete an [advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md) object.|
|[Update advancedThreatProtectionOnboardingDeviceSettingStates](../api/advancedthreatprotectiononboardingstatesummary-update-advancedthreatprotectiononboardingdevicesettingstates.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md)|Update the properties of an advancedThreatProtectionOnboardingDeviceSettingStates object.|
|[Get advancedThreatProtectionOnboardingDeviceSettingState](../api/advancedthreatprotectiononboardingdevicesettingstate-get.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md)|Read the properties and relationships of an [advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantDeviceCount|Int32|Number of compliant devices|
|conflictDeviceCount|Int32|Number of conflict devices|
|errorDeviceCount|Int32|Number of error devices|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|nonCompliantDeviceCount|Int32|Number of NonCompliant devices|
|notApplicableDeviceCount|Int32|Number of not applicable devices|
|notAssignedDeviceCount|Int32|Number of not assigned devices|
|remediatedDeviceCount|Int32|Number of remediated devices|
|unknownDeviceCount|Int32|Number of unknown devices|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|advancedThreatProtectionOnboardingDeviceSettingStates|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md) collection|**TODO: Add Description**|

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

