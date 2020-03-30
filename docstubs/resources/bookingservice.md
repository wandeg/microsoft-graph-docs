---
title: "bookingService resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# bookingService resource type


Namespace: microsoft.graph




Inherits from [bookingNamedEntity](../resources/bookingnamedentity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get bookingService](../api/bookingservice-get.md)|[bookingService](../resources/bookingservice.md)|Read properties and relationships of the [bookingService](../resources/bookingservice.md) object.|
|[Update bookingService](../api/bookingservice-update.md)|[bookingService](../resources/bookingservice.md)|Update the properties of a [bookingService](../resources/bookingservice.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|defaultDuration|Duration||
|defaultLocation|[location](../resources/location.md)||
|defaultPrice|Double||
|defaultPriceType|Enumeration| Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|defaultReminders|[bookingReminder](../resources/bookingreminder.md) collection||
|description|String||
|displayName|String| Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isHiddenFromCustomers|Boolean||
|notes|String||
|postBuffer|Duration||
|preBuffer|Duration||
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)||
|staffMemberIds|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingService",
  "baseType": "microsoft.graph.bookingNamedEntity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingService",
  "id": "String (identifier)",
  "displayName": "String",
  "defaultDuration": "String (duration)",
  "defaultLocation": {
    "@odata.type": "microsoft.graph.location"
  },
  "defaultPrice": "Double",
  "defaultPriceType": "String",
  "defaultReminders": [
    {
      "@odata.type": "microsoft.graph.bookingReminder"
    }
  ],
  "description": "String",
  "isHiddenFromCustomers": true,
  "notes": "String",
  "preBuffer": "String (duration)",
  "postBuffer": "String (duration)",
  "schedulingPolicy": {
    "@odata.type": "microsoft.graph.bookingSchedulingPolicy"
  },
  "staffMemberIds": [
    "String"
  ]
}
```

