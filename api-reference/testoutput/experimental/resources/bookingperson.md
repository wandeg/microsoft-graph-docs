---
title: "bookingPerson resource type"
description: "Represents a booking customer or staff member."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# bookingPerson resource type

Represents a booking customer or staff member.


Inherits from [bookingNamedEntity](../resources/bookingNamedEntity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List bookingPersons](../api/bookingperson-list.md)|[bookingPerson](../resources/bookingPerson.md) collection|List properties and relationships of the [bookingPerson](../resources/bookingperson.md) objects.|
|[Get bookingPerson](../api/bookingperson-get.md)|[bookingPerson](../resources/bookingPerson.md)|Read properties and relationships of the [bookingPerson](../resources/bookingperson.md) object.|
|[Create bookingPerson](../api/bookingperson-create.md)|[bookingPerson](../resources/bookingPerson.md)|Create a new [bookingPerson](../resources/bookingperson.md) object.|
|[Delete bookingPerson](../api/bookingperson-delete.md)|None|Deletes a [bookingPerson](../resources/bookingperson.md).|
|[Update bookingPerson](../api/bookingperson-update.md)|[bookingPerson](../resources/bookingPerson.md)|Update the properties of a [bookingPerson](../resources/bookingperson.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|Display name of this entity.
The display name is suitable for human-readable interfaces. Inherited from [bookingNamedEntity](../resources/bookingNamedEntity.md)|
|emailAddress|String|The e-mail address of this person.|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingPerson",
  "baseType": "microsoft.graph.bookingNamedEntity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingPerson",
  "id": "String (identifier)",
  "displayName": "String",
  "emailAddress": "String"
}
```

