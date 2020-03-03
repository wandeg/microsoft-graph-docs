---
title: "room resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# room resource type




Inherits from [place](../resources/place.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get room](../api/room-get.md)|[room](../resources/room.md)|Read properties and relationships of the [room](../resources/room.md) object.|
|[Delete room](../api/room-delete.md)|None|Deletes a [room](../resources/room.md).|
|[Update room](../api/room-update.md)|[room](../resources/room.md)|Update the properties of a [room](../resources/room.md) object.|
|[List rooms](../api/roomlist-list-rooms.md)|[room](../resources/room.md) collection|Get the rooms from the rooms navigation property.|
|[Add rooms](../api/roomlist-post-rooms.md)|[room](../resources/room.md)|Add rooms by posting to the rooms collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[physicalAddress](../resources/physicalAddress.md)| Inherited from [place](../resources/place.md)|
|audioDeviceName|String||
|bookingType|Enumeration|. Possible values are: `unknown`, `standard`, `reserved`.|
|building|String||
|capacity|Int32||
|displayDeviceName|String||
|displayName|String| Inherited from [place](../resources/place.md)|
|emailAddress|String||
|floorLabel|String||
|floorNumber|Int32||
|geoCoordinates|[outlookGeoCoordinates](../resources/outlookGeoCoordinates.md)| Inherited from [place](../resources/place.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isWheelChairAccessible|Boolean||
|label|String||
|nickname|String||
|phone|String| Inherited from [place](../resources/place.md)|
|tags|String collection||
|videoDeviceName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.room",
  "baseType": "microsoft.graph.place",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.room",
  "id": "String (identifier)",
  "displayName": "String",
  "geoCoordinates": {
    "@odata.type": "microsoft.graph.outlookGeoCoordinates"
  },
  "phone": "String",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "emailAddress": "String",
  "nickname": "String",
  "building": "String",
  "floorNumber": 1024,
  "label": "String",
  "capacity": 1024,
  "bookingType": "String",
  "audioDeviceName": "String",
  "videoDeviceName": "String",
  "displayDeviceName": "String",
  "isWheelChairAccessible": true,
  "tags": [
    "String"
  ],
  "floorLabel": "String"
}
```

