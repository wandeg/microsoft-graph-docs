---
title: "itemAnalytics resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# itemAnalytics resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get itemAnalytics](../api/itemanalytics-get.md)|[itemAnalytics](../resources/itemanalytics.md)|Read properties and relationships of an [itemAnalytics](../resources/itemanalytics.md) object.|
|[Update itemAnalytics](../api/itemanalytics-update.md)|[itemAnalytics](../resources/itemanalytics.md)|Update the properties of a [itemAnalytics](../resources/itemanalytics.md) object.|
|[List itemActivityStats](../api/itemanalytics-list-itemactivitystats.md)|[itemActivityStat](../resources/itemactivitystat.md) collection|Get the itemActivityStats from the itemActivityStats navigation property.|
|[Create itemActivityStats](../api/itemanalytics-post-itemactivitystats.md)|[itemActivityStat](../resources/itemactivitystat.md)|Create a new itemActivityStats object.|
|[Delete itemActivityStats](../api/itemanalytics-delete-itemactivitystats.md)|None|Delete an itemActivityStats object.|
|[Update itemActivityStats](../api/itemanalytics-update-itemactivitystats.md)|[itemActivityStat](../resources/itemactivitystat.md)|Update the properties of an itemActivityStats object.|
|[Get itemActivityStat](../api/itemactivitystat-get.md)|[itemActivityStat](../resources/itemactivitystat.md)|Read properties and relationships of an [itemActivityStat](../resources/itemactivitystat.md) object.|
|[List allTime](../api/itemanalytics-list-alltime.md)|[itemActivityStat](../resources/itemactivitystat.md) collection|Get the itemActivityStats from the allTime navigation property.|
|[Add allTime](../api/itemanalytics-post-alltime.md)|[itemActivityStat](../resources/itemactivitystat.md)|Add allTime by posting to the allTime collection.|
|[Remove allTime](../api/itemanalytics-delete-alltime.md)|None|Remove an allTime object.|
|[List lastSevenDays](../api/itemanalytics-list-lastsevendays.md)|[itemActivityStat](../resources/itemactivitystat.md) collection|Get the itemActivityStats from the lastSevenDays navigation property.|
|[Add lastSevenDays](../api/itemanalytics-post-lastsevendays.md)|[itemActivityStat](../resources/itemactivitystat.md)|Add lastSevenDays by posting to the lastSevenDays collection.|
|[Remove lastSevenDays](../api/itemanalytics-delete-lastsevendays.md)|None|Remove a lastSevenDays object.|
|[List analytics](../api/site-list-analytics.md)|[itemAnalytics](../resources/itemanalytics.md) collection|Get the itemAnalytics from the analytics navigation property.|
|[Add analytics](../api/site-post-analytics.md)|[itemAnalytics](../resources/itemanalytics.md)|Add analytics by posting to the analytics collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|allTime|[itemActivityStat](../resources/itemactivitystat.md)|**TODO: Add Description**|
|itemActivityStats|[itemActivityStat](../resources/itemactivitystat.md) collection|**TODO: Add Description**|
|lastSevenDays|[itemActivityStat](../resources/itemactivitystat.md)|**TODO: Add Description**|

## JSON representation
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

