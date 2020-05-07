---
title: "deviceManagementSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementSettings resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|androidDeviceAdministratorEnrollmentEnabled|Boolean|**TODO: Add Description**|
|derivedCredentialProvider|derivedCredentialProviderType|**TODO: Add Description**. Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.|
|derivedCredentialUrl|String|**TODO: Add Description**|
|deviceComplianceCheckinThresholdDays|Int32|**TODO: Add Description**|
|deviceInactivityBeforeRetirementInDay|Int32|**TODO: Add Description**|
|enhancedJailBreak|Boolean|**TODO: Add Description**|
|ignoreDevicesForUnsupportedSettingsEnabled|Boolean|**TODO: Add Description**|
|isScheduledActionEnabled|Boolean|**TODO: Add Description**|
|secureByDefault|Boolean|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": "Integer",
  "isScheduledActionEnabled": "Boolean",
  "secureByDefault": "Boolean",
  "enhancedJailBreak": "Boolean",
  "deviceInactivityBeforeRetirementInDay": "Integer",
  "derivedCredentialProvider": "String",
  "derivedCredentialUrl": "String",
  "androidDeviceAdministratorEnrollmentEnabled": "Boolean",
  "ignoreDevicesForUnsupportedSettingsEnabled": "Boolean"
}
```

