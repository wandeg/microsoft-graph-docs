---
title: "teamsUserActivityCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# teamsUserActivityCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List teamsUserActivityCountses](../api/teamsuseractivitycounts-list.md)|[teamsUserActivityCounts](../resources/teamsUserActivityCounts.md) collection|List properties and relationships of the [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) objects.|
|[Get teamsUserActivityCounts](../api/teamsuseractivitycounts-get.md)|[teamsUserActivityCounts](../resources/teamsUserActivityCounts.md)|Read properties and relationships of the [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) object.|
|[Create teamsUserActivityCounts](../api/teamsuseractivitycounts-create.md)|[teamsUserActivityCounts](../resources/teamsUserActivityCounts.md)|Create a new [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) object.|
|[Delete teamsUserActivityCounts](../api/teamsuseractivitycounts-delete.md)|None|Deletes a [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md).|
|[Update teamsUserActivityCounts](../api/teamsuseractivitycounts-update.md)|[teamsUserActivityCounts](../resources/teamsUserActivityCounts.md)|Update the properties of a [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|calls|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|meetings|Int64||
|privateChatMessages|Int64||
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|teamChatMessages|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsUserActivityCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsUserActivityCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "teamChatMessages": 1024,
  "privateChatMessages": 1024,
  "calls": 1024,
  "meetings": 1024,
  "reportPeriod": "String"
}
```

