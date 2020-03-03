---
title: "roomList resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# roomList resource type




Inherits from [place](../resources/place.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List roomLists](../api/roomlist-list.md)|[roomList](../resources/roomList.md) collection|List properties and relationships of the [roomList](../resources/roomlist.md) objects.|
|[Get roomList](../api/roomlist-get.md)|[roomList](../resources/roomList.md)|Read properties and relationships of the [roomList](../resources/roomlist.md) object.|
|[Create roomList](../api/roomlist-create.md)|[roomList](../resources/roomList.md)|Create a new [roomList](../resources/roomlist.md) object.|
|[Delete roomList](../api/roomlist-delete.md)|None|Deletes a [roomList](../resources/roomlist.md).|
|[Update roomList](../api/roomlist-update.md)|[roomList](../resources/roomList.md)|Update the properties of a [roomList](../resources/roomlist.md) object.|
|[List rooms](../api/roomlist-list-rooms.md)|[room](../resources/room.md) collection|Get the rooms from the rooms navigation property.|
|[Add rooms](../api/roomlist-post-rooms.md)|[room](../resources/room.md)|Add rooms by posting to the rooms collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[physicalAddress](../resources/physicalAddress.md)| Inherited from [place](../resources/place.md)|
|displayName|String| Inherited from [place](../resources/place.md)|
|emailAddress|String||
|geoCoordinates|[outlookGeoCoordinates](../resources/outlookGeoCoordinates.md)| Inherited from [place](../resources/place.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|phone|String| Inherited from [place](../resources/place.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|rooms|[room](../resources/room.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roomList",
  "baseType": "microsoft.graph.place",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roomList",
  "id": "String (identifier)",
  "displayName": "String",
  "geoCoordinates": {
    "@odata.type": "microsoft.graph.outlookGeoCoordinates"
  },
  "phone": "String",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "emailAddress": "String"
}
```

