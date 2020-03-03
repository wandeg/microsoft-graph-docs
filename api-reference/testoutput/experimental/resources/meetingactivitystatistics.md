---
title: "meetingActivityStatistics resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# meetingActivityStatistics resource type


Namespace: microsoft.graph




Inherits from [activityStatistics](../resources/activitystatistics.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List meetingActivityStatisticses](../api/meetingactivitystatistics-list.md)|[meetingActivityStatistics](../resources/meetingactivitystatistics.md) collection|List properties and relationships of the [meetingActivityStatistics](../resources/meetingactivitystatistics.md) objects.|
|[Get meetingActivityStatistics](../api/meetingactivitystatistics-get.md)|[meetingActivityStatistics](../resources/meetingactivitystatistics.md)|Read properties and relationships of the [meetingActivityStatistics](../resources/meetingactivitystatistics.md) object.|
|[Create meetingActivityStatistics](../api/meetingactivitystatistics-create.md)|[meetingActivityStatistics](../resources/meetingactivitystatistics.md)|Create a new [meetingActivityStatistics](../resources/meetingactivitystatistics.md) object.|
|[Delete meetingActivityStatistics](../api/meetingactivitystatistics-delete.md)|None|Deletes a [meetingActivityStatistics](../resources/meetingactivitystatistics.md).|
|[Update meetingActivityStatistics](../api/meetingactivitystatistics-update.md)|[meetingActivityStatistics](../resources/meetingactivitystatistics.md)|Update the properties of a [meetingActivityStatistics](../resources/meetingactivitystatistics.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activity|Enumeration| Inherited from [activityStatistics](../resources/activitystatistics.md). Possible values are: `Email`, `Meeting`, `Focus`, `Chat`, `Call`.|
|afterHours|Duration||
|conflicting|Duration||
|duration|Duration| Inherited from [activityStatistics](../resources/activitystatistics.md)|
|endDate|Date| Inherited from [activityStatistics](../resources/activitystatistics.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|long|Duration||
|multitasking|Duration||
|organized|Duration||
|recurring|Duration||
|startDate|Date| Inherited from [activityStatistics](../resources/activitystatistics.md)|
|timeZoneUsed|String| Inherited from [activityStatistics](../resources/activitystatistics.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.meetingActivityStatistics",
  "baseType": "microsoft.graph.activityStatistics",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.meetingActivityStatistics",
  "id": "String (identifier)",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "String",
  "duration": "String (duration)",
  "afterHours": "String (duration)",
  "organized": "String (duration)",
  "recurring": "String (duration)",
  "long": "String (duration)",
  "conflicting": "String (duration)",
  "multitasking": "String (duration)"
}
```

