---
title: "teamsUserActivityUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# teamsUserActivityUserCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List teamsUserActivityUserCountses](../api/teamsuseractivityusercounts-list.md)|[teamsUserActivityUserCounts](../resources/teamsUserActivityUserCounts.md) collection|List properties and relationships of the [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) objects.|
|[Get teamsUserActivityUserCounts](../api/teamsuseractivityusercounts-get.md)|[teamsUserActivityUserCounts](../resources/teamsUserActivityUserCounts.md)|Read properties and relationships of the [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) object.|
|[Create teamsUserActivityUserCounts](../api/teamsuseractivityusercounts-create.md)|[teamsUserActivityUserCounts](../resources/teamsUserActivityUserCounts.md)|Create a new [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) object.|
|[Delete teamsUserActivityUserCounts](../api/teamsuseractivityusercounts-delete.md)|None|Deletes a [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md).|
|[Update teamsUserActivityUserCounts](../api/teamsuseractivityusercounts-update.md)|[teamsUserActivityUserCounts](../resources/teamsUserActivityUserCounts.md)|Update the properties of a [teamsUserActivityUserCounts](../resources/teamsuseractivityusercounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|calls|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|meetings|Int64||
|otherActions|Int64||
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
  "@odata.type": "microsoft.graph.teamsUserActivityUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsUserActivityUserCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "teamChatMessages": 1024,
  "privateChatMessages": 1024,
  "calls": 1024,
  "meetings": 1024,
  "otherActions": 1024,
  "reportPeriod": "String"
}
```

