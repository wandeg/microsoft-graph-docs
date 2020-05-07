---
title: "userExperienceAnalyticsDeviceStartupHistory resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userExperienceAnalyticsDeviceStartupHistory resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|coreBootTimeInMs|Int32|**TODO: Add Description**|
|coreLoginTimeInMs|Int32|**TODO: Add Description**|
|deviceId|String|**TODO: Add Description**|
|featureUpdateBootTimeInMs|Int32|**TODO: Add Description**|
|groupPolicyBootTimeInMs|Int32|**TODO: Add Description**|
|groupPolicyLoginTimeInMs|Int32|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isFeatureUpdate|Boolean|**TODO: Add Description**|
|isFirstLogin|Boolean|**TODO: Add Description**|
|operatingSystemVersion|String|**TODO: Add Description**|
|responsiveDesktopTimeInMs|Int32|**TODO: Add Description**|
|startTime|DateTimeOffset|**TODO: Add Description**|
|totalBootTimeInMs|Int32|**TODO: Add Description**|
|totalLoginTimeInMs|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "coreBootTimeInMs": "Integer",
  "groupPolicyBootTimeInMs": "Integer",
  "featureUpdateBootTimeInMs": "Integer",
  "totalBootTimeInMs": "Integer",
  "groupPolicyLoginTimeInMs": "Integer",
  "coreLoginTimeInMs": "Integer",
  "responsiveDesktopTimeInMs": "Integer",
  "totalLoginTimeInMs": "Integer",
  "isFirstLogin": "Boolean",
  "isFeatureUpdate": "Boolean",
  "operatingSystemVersion": "String"
}
```

