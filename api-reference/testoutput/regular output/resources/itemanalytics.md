---
title: "itemAnalytics resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# itemAnalytics resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List itemAnalyticses](../api/itemanalytics-list.md)|[itemAnalytics](../resources/itemAnalytics.md) collection|List properties and relationships of the [itemAnalytics](../resources/itemanalytics.md) objects.|
|[Get itemAnalytics](../api/itemanalytics-get.md)|[itemAnalytics](../resources/itemAnalytics.md)|Read properties and relationships of the [itemAnalytics](../resources/itemanalytics.md) object.|
|[Create itemAnalytics](../api/itemanalytics-create.md)|[itemAnalytics](../resources/itemAnalytics.md)|Create a new [itemAnalytics](../resources/itemanalytics.md) object.|
|[Delete itemAnalytics](../api/itemanalytics-delete.md)|None|Deletes a [itemAnalytics](../resources/itemanalytics.md).|
|[Update itemAnalytics](../api/itemanalytics-update.md)|[itemAnalytics](../resources/itemAnalytics.md)|Update the properties of a [itemAnalytics](../resources/itemanalytics.md) object.|
|[List itemActivityStats](../api/itemanalytics-list-itemactivitystats.md)|[itemActivityStat](../resources/itemActivityStat.md) collection|Get the itemActivityStats from the itemActivityStats navigation property.|
|[Add itemActivityStats](../api/itemanalytics-post-itemactivitystats.md)|[itemActivityStat](../resources/itemActivityStat.md)|Add itemActivityStats by posting to the itemActivityStats collection.|
|[Get itemActivityStat](../api/itemactivitystat-get.md)|[itemActivityStat](../resources/itemActivityStat.md)|Read properties and relationships of the [itemActivityStat](../resources/itemactivitystat.md) object.|
|[Get itemActivityStat](../api/itemactivitystat-get.md)|[itemActivityStat](../resources/itemActivityStat.md)|Read properties and relationships of the [itemActivityStat](../resources/itemactivitystat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|allTime|[itemActivityStat](../resources/itemActivityStat.md)||
|itemActivityStats|[itemActivityStat](../resources/itemActivityStat.md) collection||
|lastSevenDays|[itemActivityStat](../resources/itemActivityStat.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemAnalytics",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemAnalytics",
  "id": "String (identifier)"
}
```

