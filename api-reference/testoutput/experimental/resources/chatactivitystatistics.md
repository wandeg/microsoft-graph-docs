---
title: "chatActivityStatistics resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# chatActivityStatistics resource type




Inherits from [activityStatistics](../resources/activityStatistics.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List chatActivityStatisticses](../api/chatactivitystatistics-list.md)|[chatActivityStatistics](../resources/chatActivityStatistics.md) collection|List properties and relationships of the [chatActivityStatistics](../resources/chatactivitystatistics.md) objects.|
|[Get chatActivityStatistics](../api/chatactivitystatistics-get.md)|[chatActivityStatistics](../resources/chatActivityStatistics.md)|Read properties and relationships of the [chatActivityStatistics](../resources/chatactivitystatistics.md) object.|
|[Create chatActivityStatistics](../api/chatactivitystatistics-create.md)|[chatActivityStatistics](../resources/chatActivityStatistics.md)|Create a new [chatActivityStatistics](../resources/chatactivitystatistics.md) object.|
|[Delete chatActivityStatistics](../api/chatactivitystatistics-delete.md)|None|Deletes a [chatActivityStatistics](../resources/chatactivitystatistics.md).|
|[Update chatActivityStatistics](../api/chatactivitystatistics-update.md)|[chatActivityStatistics](../resources/chatActivityStatistics.md)|Update the properties of a [chatActivityStatistics](../resources/chatactivitystatistics.md) object.|

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
  "@odata.type": "microsoft.graph.chatActivityStatistics",
  "baseType": "microsoft.graph.activityStatistics",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatActivityStatistics",
  "id": "String (identifier)",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "String",
  "duration": "String (duration)",
  "afterHours": "String (duration)"
}
```

