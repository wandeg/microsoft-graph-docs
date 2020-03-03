---
title: "skypeForBusinessActivityCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# skypeForBusinessActivityCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List skypeForBusinessActivityCountses](../api/skypeforbusinessactivitycounts-list.md)|[skypeForBusinessActivityCounts](../resources/skypeForBusinessActivityCounts.md) collection|List properties and relationships of the [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) objects.|
|[Get skypeForBusinessActivityCounts](../api/skypeforbusinessactivitycounts-get.md)|[skypeForBusinessActivityCounts](../resources/skypeForBusinessActivityCounts.md)|Read properties and relationships of the [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) object.|
|[Create skypeForBusinessActivityCounts](../api/skypeforbusinessactivitycounts-create.md)|[skypeForBusinessActivityCounts](../resources/skypeForBusinessActivityCounts.md)|Create a new [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) object.|
|[Delete skypeForBusinessActivityCounts](../api/skypeforbusinessactivitycounts-delete.md)|None|Deletes a [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md).|
|[Update skypeForBusinessActivityCounts](../api/skypeforbusinessactivitycounts-update.md)|[skypeForBusinessActivityCounts](../resources/skypeForBusinessActivityCounts.md)|Update the properties of a [skypeForBusinessActivityCounts](../resources/skypeforbusinessactivitycounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|organized|Int64||
|participated|Int64||
|peerToPeer|Int64||
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeForBusinessActivityCounts",
  "id": "String (identifier)",
  "peerToPeer": 1024,
  "organized": 1024,
  "participated": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

