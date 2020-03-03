---
title: "userExperienceAnalyticsDeviceStartupHistory resource type"
description: "The user experience analytics device startup history entity contains device boot performance history details."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userExperienceAnalyticsDeviceStartupHistory resource type


Namespace: microsoft.graph

The user experience analytics device startup history entity contains device boot performance history details.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List userExperienceAnalyticsDeviceStartupHistories](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-list.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) collection|List properties and relationships of the [userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md) objects.|
|[Get userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-get.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Read properties and relationships of the [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.|
|[Create userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-create.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Create a new [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.|
|[Delete userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-delete.md)|None|Deletes a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md).|
|[Update userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-userexperienceanalyticsdevicestartuphistory-update.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Update the properties of a [userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) object.|
|[List userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-devicemanagement-list-userexperienceanalyticsdevicestartuphistory.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md) collection|Get the userExperienceAnalyticsDeviceStartupHistories from the userExperienceAnalyticsDeviceStartupHistory navigation property.|
|[Add userExperienceAnalyticsDeviceStartupHistory](../api/intune-devices-devicemanagement-post-userexperienceanalyticsdevicestartuphistory.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/intune-devices-userexperienceanalyticsdevicestartuphistory.md)|Add userExperienceAnalyticsDeviceStartupHistory by posting to the userExperienceAnalyticsDeviceStartupHistory collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|coreBootTimeInMs|Int32|The user experience analytics device core boot time in milliseconds.|
|coreLoginTimeInMs|Int32|The user experience analytics device core login time in milliseconds.|
|deviceId|String|The user experience analytics device id.|
|featureUpdateBootTimeInMs|Int32|The user experience analytics device feature update time in milliseconds.|
|groupPolicyBootTimeInMs|Int32|The User experience analytics Device group policy boot time in milliseconds.|
|groupPolicyLoginTimeInMs|Int32|The User experience analytics Device group policy login time in milliseconds.|
|id|String| Inherited from [entity](../resources/entity.md)|
|isFeatureUpdate|Boolean|The user experience analytics device boot record is a feature update.|
|isFirstLogin|Boolean|The user experience analytics device first login.|
|operatingSystemVersion|String|The user experience analytics device boot record's operating system version.|
|startTime|DateTimeOffset|The user experience analytics device boot start time.|
|totalBootTimeInMs|Int32|The user experience analytics device total boot time in milliseconds.|
|totalLoginTimeInMs|Int32|The user experience analytics device total login time in milliseconds.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupHistory",
  "id": "String (identifier)",
  "deviceId": "String",
  "startTime": "String (timestamp)",
  "coreBootTimeInMs": 1024,
  "groupPolicyBootTimeInMs": 1024,
  "featureUpdateBootTimeInMs": 1024,
  "totalBootTimeInMs": 1024,
  "groupPolicyLoginTimeInMs": 1024,
  "coreLoginTimeInMs": 1024,
  "totalLoginTimeInMs": 1024,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "String"
}
```

