---
title: "roomList resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# roomList resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [place](../resources/place.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List rooms](../api/roomlist-list-rooms.md)|[room](../resources/room.md) collection|Get the rooms from the rooms navigation property.|
|[Create rooms](../api/roomlist-post-rooms.md)|[room](../resources/room.md)|Create a new rooms object.|
|[Delete rooms](../api/roomlist-delete-rooms.md)|None|Delete a [room](../resources/room.md) object.|
|[Update rooms](../api/roomlist-update-rooms.md)|[room](../resources/room.md)|Update the properties of a rooms object.|
|[Get rooms](../api/roomlist-get-room.md)|[room](../resources/room.md)|Read the properties and relationships of a [room](../resources/room.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description** Inherited from [place](../resources/place.md)|
|displayName|String|**TODO: Add Description** Inherited from [place](../resources/place.md)|
|emailAddress|String|**TODO: Add Description**|
|geoCoordinates|[outlookGeoCoordinates](../resources/outlookgeocoordinates.md)|**TODO: Add Description** Inherited from [place](../resources/place.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|phone|String|**TODO: Add Description** Inherited from [place](../resources/place.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|rooms|[room](../resources/room.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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

