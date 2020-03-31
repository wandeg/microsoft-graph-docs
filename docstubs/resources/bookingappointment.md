---
title: "bookingAppointment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# bookingAppointment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get bookingAppointment](../api/bookingappointment-get.md)|[bookingAppointment](../resources/bookingappointment.md)|Read properties and relationships of the [bookingAppointment](../resources/bookingappointment.md) object.|
|[Update bookingAppointment](../api/bookingappointment-update.md)|[bookingAppointment](../resources/bookingappointment.md)|Update the properties of a [bookingAppointment](../resources/bookingappointment.md) object.|
|[cancel](../api/bookingappointment-cancel.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|customerEmailAddress|String||
|customerId|String||
|customerLocation|[location](../resources/location.md)||
|customerName|String||
|customerNotes|String||
|customerPhone|String||
|duration|Duration||
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|invoiceAmount|Double||
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|invoiceId|String||
|invoiceStatus|Enumeration| Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|String||
|optOutOfCustomerEmail|Boolean||
|postBuffer|Duration||
|preBuffer|Duration||
|price|Double||
|priceType|Enumeration| Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|reminders|[bookingReminder](../resources/bookingreminder.md) collection||
|selfServiceAppointmentId|String||
|serviceId|String||
|serviceLocation|[location](../resources/location.md)||
|serviceName|String||
|serviceNotes|String||
|staffMemberIds|String collection||
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingAppointment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingAppointment",
  "id": "String (identifier)",
  "selfServiceAppointmentId": "String",
  "customerId": "String",
  "customerName": "String",
  "customerEmailAddress": "String",
  "customerPhone": "String",
  "customerLocation": {
    "@odata.type": "microsoft.graph.location"
  },
  "customerNotes": "String",
  "serviceId": "String",
  "serviceName": "String",
  "start": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "end": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "duration": "String (duration)",
  "preBuffer": "String (duration)",
  "postBuffer": "String (duration)",
  "serviceLocation": {
    "@odata.type": "microsoft.graph.location"
  },
  "priceType": "String",
  "price": "Double",
  "serviceNotes": "String",
  "reminders": [
    {
      "@odata.type": "microsoft.graph.bookingReminder"
    }
  ],
  "optOutOfCustomerEmail": true,
  "staffMemberIds": [
    "String"
  ],
  "invoiceAmount": "Double",
  "invoiceDate": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "invoiceId": "String",
  "invoiceStatus": "String",
  "invoiceUrl": "String"
}
```

