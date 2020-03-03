---
title: "bookingNamedEntity resource type"
description: "Booking entities that provide a display name."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# bookingNamedEntity resource type

Booking entities that provide a display name.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List bookingNamedEntities](../api/bookingnamedentity-list.md)|[bookingNamedEntity](../resources/bookingNamedEntity.md) collection|List properties and relationships of the [bookingNamedEntity](../resources/bookingnamedentity.md) objects.|
|[Get bookingNamedEntity](../api/bookingnamedentity-get.md)|[bookingNamedEntity](../resources/bookingNamedEntity.md)|Read properties and relationships of the [bookingNamedEntity](../resources/bookingnamedentity.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|Display name of this entity.
The display name is suitable for human-readable interfaces.|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingNamedEntity",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingNamedEntity",
  "id": "String (identifier)",
  "displayName": "String"
}
```

