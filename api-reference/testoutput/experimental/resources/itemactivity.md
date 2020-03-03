---
title: "itemActivity resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# itemActivity resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get itemActivity](../api/itemactivity-get.md)|[itemActivity](../resources/itemActivity.md)|Read properties and relationships of the [itemActivity](../resources/itemactivity.md) object.|
|[Delete itemActivity](../api/itemactivity-delete.md)|None|Deletes a [itemActivity](../resources/itemactivity.md).|
|[Update itemActivity](../api/itemactivity-update.md)|[itemActivity](../resources/itemActivity.md)|Update the properties of a [itemActivity](../resources/itemactivity.md) object.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveItem.md)|Read properties and relationships of the [driveItem](../resources/driveitem.md) object.|
|[List activities](../api/itemactivitystat-list-activities.md)|[itemActivity](../resources/itemActivity.md) collection|Get the itemActivities from the activities navigation property.|
|[Create activities](../api/itemactivitystat-post-activities.md)|[itemActivity](../resources/itemActivity.md)|Create activities by posting to the activities collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|access|[accessAction](../resources/accessAction.md)||
|activityDateTime|DateTimeOffset||
|actor|[identitySet](../resources/identitySet.md)||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|driveItem|[driveItem](../resources/driveItem.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemActivity",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemActivity",
  "id": "String (identifier)",
  "access": {
    "@odata.type": "microsoft.graph.accessAction"
  },
  "activityDateTime": "String (timestamp)",
  "actor": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

