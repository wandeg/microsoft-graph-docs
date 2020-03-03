---
title: "focusActivityStatistics resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# focusActivityStatistics resource type


Namespace: microsoft.graph




Inherits from [activityStatistics](../resources/activitystatistics.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List focusActivityStatisticses](../api/focusactivitystatistics-list.md)|[focusActivityStatistics](../resources/focusactivitystatistics.md) collection|List properties and relationships of the [focusActivityStatistics](../resources/focusactivitystatistics.md) objects.|
|[Get focusActivityStatistics](../api/focusactivitystatistics-get.md)|[focusActivityStatistics](../resources/focusactivitystatistics.md)|Read properties and relationships of the [focusActivityStatistics](../resources/focusactivitystatistics.md) object.|
|[Create focusActivityStatistics](../api/focusactivitystatistics-create.md)|[focusActivityStatistics](../resources/focusactivitystatistics.md)|Create a new [focusActivityStatistics](../resources/focusactivitystatistics.md) object.|
|[Delete focusActivityStatistics](../api/focusactivitystatistics-delete.md)|None|Deletes a [focusActivityStatistics](../resources/focusactivitystatistics.md).|
|[Update focusActivityStatistics](../api/focusactivitystatistics-update.md)|[focusActivityStatistics](../resources/focusactivitystatistics.md)|Update the properties of a [focusActivityStatistics](../resources/focusactivitystatistics.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activity|Enumeration| Inherited from [activityStatistics](../resources/activitystatistics.md). Possible values are: `Email`, `Meeting`, `Focus`, `Chat`, `Call`.|
|duration|Duration| Inherited from [activityStatistics](../resources/activitystatistics.md)|
|endDate|Date| Inherited from [activityStatistics](../resources/activitystatistics.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|startDate|Date| Inherited from [activityStatistics](../resources/activitystatistics.md)|
|timeZoneUsed|String| Inherited from [activityStatistics](../resources/activitystatistics.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.focusActivityStatistics",
  "baseType": "microsoft.graph.activityStatistics",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.focusActivityStatistics",
  "id": "String (identifier)",
  "activity": "String",
  "startDate": "Date",
  "endDate": "Date",
  "timeZoneUsed": "String",
  "duration": "String (duration)"
}
```

