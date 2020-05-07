---
title: "bookingAppointment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# bookingAppointment resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[cancel](../api/bookingappointment-cancel.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|customerEmailAddress|String|**TODO: Add Description**|
|customerId|String|**TODO: Add Description**|
|customerLocation|[location](../resources/location.md)|**TODO: Add Description**|
|customerName|String|**TODO: Add Description**|
|customerNotes|String|**TODO: Add Description**|
|customerPhone|String|**TODO: Add Description**|
|duration|Duration|**TODO: Add Description**|
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|invoiceAmount|Double|**TODO: Add Description**|
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|invoiceId|String|**TODO: Add Description**|
|invoiceStatus|bookingInvoiceStatus|**TODO: Add Description**. Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|String|**TODO: Add Description**|
|optOutOfCustomerEmail|Boolean|**TODO: Add Description**|
|postBuffer|Duration|**TODO: Add Description**|
|preBuffer|Duration|**TODO: Add Description**|
|price|Double|**TODO: Add Description**|
|priceType|bookingPriceType|**TODO: Add Description**. Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|reminders|[bookingReminder](../resources/bookingreminder.md) collection|**TODO: Add Description**|
|selfServiceAppointmentId|String|**TODO: Add Description**|
|serviceId|String|**TODO: Add Description**|
|serviceLocation|[location](../resources/location.md)|**TODO: Add Description**|
|serviceName|String|**TODO: Add Description**|
|serviceNotes|String|**TODO: Add Description**|
|staffMemberIds|String collection|**TODO: Add Description**|
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "optOutOfCustomerEmail": "Boolean",
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

