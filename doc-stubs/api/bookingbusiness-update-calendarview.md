---
title: "Update calendarView"
description: "Update the properties of a calendarView object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update calendarView

Namespace: microsoft.graph

Update the properties of a calendarView object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /bookingBusinesses/{bookingBusinessesId}/calendarView
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [bookingAppointment](../resources/bookingappointment.md) object.

The following table shows the properties that are required when you create the [bookingAppointment](../resources/bookingappointment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|selfServiceAppointmentId|String|**TODO: Add Description**|
|customerId|String|**TODO: Add Description**|
|customerName|String|**TODO: Add Description**|
|customerEmailAddress|String|**TODO: Add Description**|
|customerPhone|String|**TODO: Add Description**|
|customerLocation|[location](../resources/location.md)|**TODO: Add Description**|
|customerNotes|String|**TODO: Add Description**|
|serviceId|String|**TODO: Add Description**|
|serviceName|String|**TODO: Add Description**|
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|duration|Duration|**TODO: Add Description**|
|preBuffer|Duration|**TODO: Add Description**|
|postBuffer|Duration|**TODO: Add Description**|
|serviceLocation|[location](../resources/location.md)|**TODO: Add Description**|
|priceType|bookingPriceType|**TODO: Add Description**. Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|price|Double|**TODO: Add Description**|
|serviceNotes|String|**TODO: Add Description**|
|reminders|[bookingReminder](../resources/bookingreminder.md) collection|**TODO: Add Description**|
|optOutOfCustomerEmail|Boolean|**TODO: Add Description**|
|staffMemberIds|String collection|**TODO: Add Description**|
|invoiceAmount|Double|**TODO: Add Description**|
|invoiceDate|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|invoiceId|String|**TODO: Add Description**|
|invoiceStatus|bookingInvoiceStatus|**TODO: Add Description**. Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [bookingAppointment](../resources/bookingappointment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_calendarview"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}/calendarView
Content-Type: application/json
Content-length: 1169

{
  "@odata.type": "#microsoft.graph.bookingAppointment",
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

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.bookingAppointment",
  "id": "45c2495c-495c-45c2-5c49-c2455c49c245",
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

