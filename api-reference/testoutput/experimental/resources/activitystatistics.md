---
title: "activityStatistics resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# activityStatistics resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List activityStatisticses](../api/activitystatistics-list.md)|[activityStatistics](../resources/activitystatistics.md) collection|List properties and relationships of the [activityStatistics](../resources/activitystatistics.md) objects.|
|[Get activityStatistics](../api/activitystatistics-get.md)|[activityStatistics](../resources/activitystatistics.md)|Read properties and relationships of the [activityStatistics](../resources/activitystatistics.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activity|Enumeration|. Possible values are: `Email`, `Meeting`, `Focus`, `Chat`, `Call`.|
|duration|Duration||
|endDate|Date||
|id|String| Inherited from [entity](../resources/entity.md)|
|startDate|Date||
|timeZoneUsed|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.activityStatistics",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.activityStatistics",
  "id": "String (identifier)",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "String",
  "duration": "String (duration)"
}
```

