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
|androidDeviceAdministratorEnrollmentEnabled|Boolean|The property to determine if Android device administrator enrollment is enabled for this account.|
|derivedCredentialProvider|derivedCredentialProviderType|The Derived Credential Provider to use for this account. Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.|
|derivedCredentialUrl|String|The Derived Credential Provider self-service URI.|
|deviceComplianceCheckinThresholdDays|Int32|The number of days a device is allowed to go without checking in to remain compliant.|
|deviceInactivityBeforeRetirementInDay|Int32|When the device does not check in for specified number of days, the company data might be removed and the device will not be under management. Valid values 30 to 270|
|enhancedJailBreak|Boolean|Is feature enabled or not for enhanced jailbreak detection.|
|ignoreDevicesForUnsupportedSettingsEnabled|Boolean|The property to determine whether to ignore unsupported compliance settings on certian models of devices.|
|isScheduledActionEnabled|Boolean|Is feature enabled or not for scheduled action for rule.|
|secureByDefault|Boolean|Device should be noncompliant when there is no compliance policy targeted when this is true|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true,
  "enhancedJailBreak": true,
  "deviceInactivityBeforeRetirementInDay": 1024,
  "derivedCredentialProvider": "String",
  "derivedCredentialUrl": "String",
  "androidDeviceAdministratorEnrollmentEnabled": true,
  "ignoreDevicesForUnsupportedSettingsEnabled": true
}
```

