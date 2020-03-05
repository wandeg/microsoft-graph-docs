---
title: "itemActivityStat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# itemActivityStat resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List itemActivityStats](../api/itemactivitystat-list.md)|[itemActivityStat](../resources/itemactivitystat.md) collection|List properties and relationships of the [itemActivityStat](../resources/itemactivitystat.md) objects.|
|[Get itemActivityStat](../api/itemactivitystat-get.md)|[itemActivityStat](../resources/itemactivitystat.md)|Read properties and relationships of the [itemActivityStat](../resources/itemactivitystat.md) object.|
|[Create itemActivityStat](../api/itemactivitystat-create.md)|[itemActivityStat](../resources/itemactivitystat.md)|Create a new [itemActivityStat](../resources/itemactivitystat.md) object.|
|[Delete itemActivityStat](../api/itemactivitystat-delete.md)|None|Deletes a [itemActivityStat](../resources/itemactivitystat.md).|
|[Update itemActivityStat](../api/itemactivitystat-update.md)|[itemActivityStat](../resources/itemactivitystat.md)|Update the properties of a [itemActivityStat](../resources/itemactivitystat.md) object.|
|[List activities](../api/itemactivitystat-list-activities.md)|[itemActivity](../resources/itemactivity.md) collection|Get the itemActivities from the activities navigation property.|
|[Create activities](../api/itemactivitystat-post-activities.md)|[itemActivity](../resources/itemactivity.md)|Create activities by posting to the activities collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|access|[itemActionStat](../resources/itemactionstat.md)||
|create|[itemActionStat](../resources/itemactionstat.md)||
|delete|[itemActionStat](../resources/itemactionstat.md)||
|edit|[itemActionStat](../resources/itemactionstat.md)||
|endDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|incompleteData|[incompleteData](../resources/incompletedata.md)||
|isTrending|Boolean||
|move|[itemActionStat](../resources/itemactionstat.md)||
|startDateTime|DateTimeOffset||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activities|[itemActivity](../resources/itemactivity.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemActivityStat",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemActivityStat",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "access": {
    "@odata.type": "microsoft.graph.itemActionStat",
    "actionCount": 1024,
    "actorCount": 1024
  },
  "create": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "delete": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "edit": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "move": {
    "@odata.type": "microsoft.graph.itemActionStat"
  },
  "isTrending": true,
  "incompleteData": {
    "@odata.type": "microsoft.graph.incompleteData",
    "missingDataBeforeDateTime": "String (timestamp)",
    "wasThrottled": true
  }
}
```

