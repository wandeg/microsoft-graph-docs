---
title: "advancedThreatProtectionOnboardingStateSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# advancedThreatProtectionOnboardingStateSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List advancedThreatProtectionOnboardingDeviceSettingStates](../api/advancedthreatprotectiononboardingstatesummary-list-advancedthreatprotectiononboardingdevicesettingstates.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md) collection|Get the advancedThreatProtectionOnboardingDeviceSettingStates from the advancedThreatProtectionOnboardingDeviceSettingStates navigation property.|
|[Create advancedThreatProtectionOnboardingDeviceSettingStates](../api/advancedthreatprotectiononboardingstatesummary-post-advancedthreatprotectiononboardingdevicesettingstates.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md)|Create a new advancedThreatProtectionOnboardingDeviceSettingStates object.|
|[Delete advancedThreatProtectionOnboardingDeviceSettingStates](../api/advancedthreatprotectiononboardingstatesummary-delete-advancedthreatprotectiononboardingdevicesettingstates.md)|None|Delete an [advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md) object.|
|[Update advancedThreatProtectionOnboardingDeviceSettingStates](../api/advancedthreatprotectiononboardingstatesummary-update-advancedthreatprotectiononboardingdevicesettingstates.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md)|Update the properties of an advancedThreatProtectionOnboardingDeviceSettingStates object.|
|[Get advancedThreatProtectionOnboardingDeviceSettingState](../api/advancedthreatprotectiononboardingdevicesettingstate-get.md)|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md)|Read the properties and relationships of an [advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantDeviceCount|Int32|**TODO: Add Description**|
|conflictDeviceCount|Int32|**TODO: Add Description**|
|errorDeviceCount|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|nonCompliantDeviceCount|Int32|**TODO: Add Description**|
|notApplicableDeviceCount|Int32|**TODO: Add Description**|
|notAssignedDeviceCount|Int32|**TODO: Add Description**|
|remediatedDeviceCount|Int32|**TODO: Add Description**|
|unknownDeviceCount|Int32|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|advancedThreatProtectionOnboardingDeviceSettingStates|[advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "unknownDeviceCount": "Integer",
  "notApplicableDeviceCount": "Integer",
  "compliantDeviceCount": "Integer",
  "remediatedDeviceCount": "Integer",
  "nonCompliantDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "conflictDeviceCount": "Integer",
  "notAssignedDeviceCount": "Integer"
}
```

