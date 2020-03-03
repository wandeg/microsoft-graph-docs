---
title: "callActivityStatistics resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# callActivityStatistics resource type




Inherits from [activityStatistics](../resources/activityStatistics.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List callActivityStatisticses](../api/callactivitystatistics-list.md)|[callActivityStatistics](../resources/callActivityStatistics.md) collection|List properties and relationships of the [callActivityStatistics](../resources/callactivitystatistics.md) objects.|
|[Get callActivityStatistics](../api/callactivitystatistics-get.md)|[callActivityStatistics](../resources/callActivityStatistics.md)|Read properties and relationships of the [callActivityStatistics](../resources/callactivitystatistics.md) object.|
|[Create callActivityStatistics](../api/callactivitystatistics-create.md)|[callActivityStatistics](../resources/callActivityStatistics.md)|Create a new [callActivityStatistics](../resources/callactivitystatistics.md) object.|
|[Delete callActivityStatistics](../api/callactivitystatistics-delete.md)|None|Deletes a [callActivityStatistics](../resources/callactivitystatistics.md).|
|[Update callActivityStatistics](../api/callactivitystatistics-update.md)|[callActivityStatistics](../resources/callActivityStatistics.md)|Update the properties of a [callActivityStatistics](../resources/callactivitystatistics.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activity|Enumeration| Inherited from [activityStatistics](../resources/activityStatistics.md). Possible values are: `Email`, `Meeting`, `Focus`, `Chat`, `Call`.|
|afterHours|Duration||
|duration|Duration| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|endDate|Date| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|startDate|Date| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|timeZoneUsed|String| Inherited from [activityStatistics](../resources/activityStatistics.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.callActivityStatistics",
  "baseType": "microsoft.graph.activityStatistics",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callActivityStatistics",
  "id": "String (identifier)",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "String",
  "duration": "String (duration)",
  "afterHours": "String (duration)"
}
```

