---
title: "userExperienceAnalyticsDeviceStartupHistory resource type"
description: "The user experience analytics device startup history entity contains device boot performance history details."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userExperienceAnalyticsDeviceStartupHistory resource type


Namespace: microsoft.graph

The user experience analytics device startup history entity contains device boot performance history details.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userExperienceAnalyticsDeviceStartupHistory](../api/userexperienceanalyticsdevicestartuphistory-get.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md)|Read the properties and relationships of a [userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md) object.|
|[Update userExperienceAnalyticsDeviceStartupHistory](../api/userexperienceanalyticsdevicestartuphistory-update.md)|[userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md)|Update the properties of a [userExperienceAnalyticsDeviceStartupHistory](../resources/userexperienceanalyticsdevicestartuphistory.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|coreBootTimeInMs|Int32|The user experience analytics device core boot time in milliseconds.|
|coreLoginTimeInMs|Int32|The user experience analytics device core login time in milliseconds.|
|deviceId|String|The user experience analytics device id.|
|featureUpdateBootTimeInMs|Int32|The user experience analytics device feature update time in milliseconds.|
|groupPolicyBootTimeInMs|Int32|The User experience analytics Device group policy boot time in milliseconds.|
|groupPolicyLoginTimeInMs|Int32|The User experience analytics Device group policy login time in milliseconds.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isFeatureUpdate|Boolean|The user experience analytics device boot record is a feature update.|
|isFirstLogin|Boolean|The user experience analytics device first login.|
|operatingSystemVersion|String|The user experience analytics device boot record's operating system version.|
|responsiveDesktopTimeInMs|Int32|The user experience analytics responsive desktop time in milliseconds.|
|startTime|DateTimeOffset|The user experience analytics device boot start time.|
|totalBootTimeInMs|Int32|The user experience analytics device total boot time in milliseconds.|
|totalLoginTimeInMs|Int32|The user experience analytics device total login time in milliseconds.|

## Relationships
None

## JSON representation
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
  "responsiveDesktopTimeInMs": 1024,
  "totalLoginTimeInMs": 1024,
  "isFirstLogin": true,
  "isFeatureUpdate": true,
  "operatingSystemVersion": "String"
}
```

