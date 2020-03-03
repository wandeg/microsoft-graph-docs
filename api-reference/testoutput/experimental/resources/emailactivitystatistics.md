---
title: "emailActivityStatistics resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# emailActivityStatistics resource type




Inherits from [activityStatistics](../resources/activityStatistics.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List emailActivityStatisticses](../api/emailactivitystatistics-list.md)|[emailActivityStatistics](../resources/emailActivityStatistics.md) collection|List properties and relationships of the [emailActivityStatistics](../resources/emailactivitystatistics.md) objects.|
|[Get emailActivityStatistics](../api/emailactivitystatistics-get.md)|[emailActivityStatistics](../resources/emailActivityStatistics.md)|Read properties and relationships of the [emailActivityStatistics](../resources/emailactivitystatistics.md) object.|
|[Create emailActivityStatistics](../api/emailactivitystatistics-create.md)|[emailActivityStatistics](../resources/emailActivityStatistics.md)|Create a new [emailActivityStatistics](../resources/emailactivitystatistics.md) object.|
|[Delete emailActivityStatistics](../api/emailactivitystatistics-delete.md)|None|Deletes a [emailActivityStatistics](../resources/emailactivitystatistics.md).|
|[Update emailActivityStatistics](../api/emailactivitystatistics-update.md)|[emailActivityStatistics](../resources/emailActivityStatistics.md)|Update the properties of a [emailActivityStatistics](../resources/emailactivitystatistics.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activity|Enumeration| Inherited from [activityStatistics](../resources/activityStatistics.md). Possible values are: `Email`, `Meeting`, `Focus`, `Chat`, `Call`.|
|afterHours|Duration||
|duration|Duration| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|endDate|Date| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|readEmail|Duration||
|sentEmail|Duration||
|startDate|Date| Inherited from [activityStatistics](../resources/activityStatistics.md)|
|timeZoneUsed|String| Inherited from [activityStatistics](../resources/activityStatistics.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailActivityStatistics",
  "baseType": "microsoft.graph.activityStatistics",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailActivityStatistics",
  "id": "String (identifier)",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "String",
  "duration": "String (duration)",
  "afterHours": "String (duration)",
  "readEmail": "String (duration)",
  "sentEmail": "String (duration)"
}
```

