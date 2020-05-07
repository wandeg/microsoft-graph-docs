---
title: "userExperienceAnalyticsDevicePerformance resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userExperienceAnalyticsDevicePerformance resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[summarizeDevicePerformanceDevices](../api/userexperienceanalyticsdeviceperformance-summarizedeviceperformancedevices.md)|[userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md) collection|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bootScore|Int32|**TODO: Add Description**|
|coreBootTimeInMs|Int32|**TODO: Add Description**|
|coreLoginTimeInMs|Int32|**TODO: Add Description**|
|deviceCount|Int64|**TODO: Add Description**|
|deviceName|String|**TODO: Add Description**|
|diskType|diskType|**TODO: Add Description**. Possible values are: `unkown`, `hdd`, `ssd`.|
|groupPolicyBootTimeInMs|Int32|**TODO: Add Description**|
|groupPolicyLoginTimeInMs|Int32|**TODO: Add Description**|
|healthStatus|userExperienceAnalyticsHealthState|**TODO: Add Description**. Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|loginScore|Int32|**TODO: Add Description**|
|manufacturer|String|**TODO: Add Description**|
|model|String|**TODO: Add Description**|
|operatingSystemVersion|String|**TODO: Add Description**|
|responsiveDesktopTimeInMs|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
  "id": "String (identifier)",
  "deviceName": "String",
  "model": "String",
  "manufacturer": "String",
  "diskType": "String",
  "operatingSystemVersion": "String",
  "bootScore": "Integer",
  "coreBootTimeInMs": "Integer",
  "groupPolicyBootTimeInMs": "Integer",
  "healthStatus": "String",
  "loginScore": "Integer",
  "coreLoginTimeInMs": "Integer",
  "groupPolicyLoginTimeInMs": "Integer",
  "deviceCount": "Integer",
  "responsiveDesktopTimeInMs": "Integer"
}
```

