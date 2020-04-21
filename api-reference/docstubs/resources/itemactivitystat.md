---
title: "itemActivityStat resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# itemActivityStat resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get itemActivityStat](../api/itemactivitystat-get.md)|[itemActivityStat](../resources/itemactivitystat.md)|Read properties and relationships of an [itemActivityStat](../resources/itemactivitystat.md) object.|
|[Update itemActivityStat](../api/itemactivitystat-update.md)|[itemActivityStat](../resources/itemactivitystat.md)|Update the properties of a [itemActivityStat](../resources/itemactivitystat.md) object.|
|[List activities](../api/itemactivitystat-list-activities.md)|[itemActivity](../resources/itemactivity.md) collection|Get the itemActivities from the activities navigation property.|
|[Add activities](../api/itemactivitystat-post-activities.md)|[itemActivity](../resources/itemactivity.md)|Add activities by posting to the activities collection.|
|[Remove activities](../api/itemactivitystat-delete-activities.md)|None|Remove an activities object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|access|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|create|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|delete|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|edit|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|incompleteData|[incompleteData](../resources/incompletedata.md)|**TODO: Add Description**|
|isTrending|Boolean|**TODO: Add Description**|
|move|[itemActionStat](../resources/itemactionstat.md)|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activities|[itemActivity](../resources/itemactivity.md) collection|**TODO: Add Description**|

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

