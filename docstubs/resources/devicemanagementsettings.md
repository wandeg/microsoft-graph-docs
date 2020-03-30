---
title: "deviceManagementSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementSettings resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|androidDeviceAdministratorEnrollmentEnabled|Boolean||
|derivedCredentialProvider|Enumeration| Possible values are: `notConfigured`, `entrustDataCard`, `purebred`, `xTec`, `intercede`.|
|derivedCredentialUrl|String||
|deviceComplianceCheckinThresholdDays|Int32||
|deviceInactivityBeforeRetirementInDay|Int32||
|enhancedJailBreak|Boolean||
|ignoreDevicesForUnsupportedSettingsEnabled|Boolean||
|isScheduledActionEnabled|Boolean||
|secureByDefault|Boolean||

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

