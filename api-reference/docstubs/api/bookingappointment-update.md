---
title: "Update bookingAppointment"
description: "Update the properties of a bookingAppointment object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update bookingAppointment

Namespace: microsoft.graph

Update the properties of a [bookingAppointment](../resources/bookingappointment.md) object.

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
PATCH /bookingBusinesses/{bookingBusinessesId}/appointments/{bookingAppointmentId}
PATCH /bookingBusinesses/{bookingBusinessesId}/calendarView/{bookingAppointmentId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [bookingAppointment](../resources/bookingappointment.md) object.

The following table shows the properties that are required when you create the [bookingAppointment](../resources/bookingappointment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|selfServiceAppointmentId|String|**TODO: Add Description**|
|customerId|String|The id of the booking customer associated with this appointment.
If CustomerId is not specified when an appointment is created then a new customer is created based on the appointment customer information. Once set, the customerId should be considered immutable.|
|customerName|String|**TODO: Add Description**|
|customerEmailAddress|String|**TODO: Add Description**|
|customerPhone|String|**TODO: Add Description**|
|customerLocation|[location](../resources/location.md)|**TODO: Add Description**|
|customerNotes|String|Notes from the customer associated with this appointment.
The value of this property is only available when reading an individual booking appointment by id. Its value can only be set when creating a new appointment with a new customer, ie, without specifying a CustomerId. After that, the property is computed from the customer represented by CustomerId.|
|serviceId|String|The id of the booking service associated with this appointment.|
|serviceName|String|The name of the booking service associated with this appointment.
This property is optional when creating a new appointment. If not specified, it is computed from the service associated with the appointment by the service id.|
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|duration|Duration|**TODO: Add Description**|
|preBuffer|Duration|**TODO: Add Description**|
|postBuffer|Duration|**TODO: Add Description**|
|serviceLocation|[location](../resources/location.md)|**TODO: Add Description**|
|priceType|bookingPriceType|**TODO: Add Description**. Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|price|Double|**TODO: Add Description**|
|serviceNotes|String|The value of this property is only available when reading an individual booking appointment by id.|
|reminders|[bookingReminder](../resources/bookingreminder.md) collection|The value of this property is only available when reading an individual booking appointment by id.|
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
  "name": "update_bookingappointment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}/appointments/{bookingAppointmentId}
Content-Type: application/json
Content-length: 2348

{
  "@odata.type": "#microsoft.graph.bookingAppointment",
  "selfServiceAppointmentId": "Self Service Appointment Id value",
  "customerId": "Customer Id value",
  "customerName": "Customer Name value",
  "customerEmailAddress": "Customer Email Address value",
  "customerPhone": "Customer Phone value",
  "customerLocation": {
    "@odata.type": "microsoft.graph.location",
    "displayName": "Display Name value",
    "locationEmailAddress": "Location Email Address value",
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress",
      "type": "String",
      "postOfficeBox": "Post Office Box value",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryOrRegion": "Country Or Region value",
      "postalCode": "Postal Code value"
    },
    "coordinates": {
      "@odata.type": "microsoft.graph.outlookGeoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double",
      "accuracy": "Double",
      "altitudeAccuracy": "Double"
    },
    "locationUri": "Location Uri value",
    "locationType": "String",
    "uniqueId": "Unique Id value",
    "uniqueIdType": "String"
  },
  "customerNotes": "Customer Notes value",
  "serviceId": "Service Id value",
  "serviceName": "Service Name value",
  "start": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "Date Time value",
    "timeZone": "Time Zone value"
  },
  "end": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "duration": "-PT0.9940994S",
  "preBuffer": "-PT36.7327427S",
  "postBuffer": "PT3M21.6931326S",
  "serviceLocation": {
    "@odata.type": "microsoft.graph.location"
  },
  "priceType": "String",
  "price": "Double",
  "serviceNotes": "Service Notes value",
  "reminders": [
    {
      "@odata.type": "microsoft.graph.bookingReminder",
      "offset": "-PT43.7329867S",
      "recipients": "String",
      "message": "Message value"
    }
  ],
  "optOutOfCustomerEmail": true,
  "staffMemberIds": [
    "Staff Member Ids value"
  ],
  "invoiceAmount": "Double",
  "invoiceDate": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "invoiceId": "Invoice Id value",
  "invoiceStatus": "String",
  "invoiceUrl": "https://example.com/invoiceUrl/"
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
  "id": "bfb28eb5-8eb5-bfb2-b58e-b2bfb58eb2bf",
  "selfServiceAppointmentId": "Self Service Appointment Id value",
  "customerId": "Customer Id value",
  "customerName": "Customer Name value",
  "customerEmailAddress": "Customer Email Address value",
  "customerPhone": "Customer Phone value",
  "customerLocation": {
    "@odata.type": "microsoft.graph.location",
    "displayName": "Display Name value",
    "locationEmailAddress": "Location Email Address value",
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress",
      "type": "String",
      "postOfficeBox": "Post Office Box value",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryOrRegion": "Country Or Region value",
      "postalCode": "Postal Code value"
    },
    "coordinates": {
      "@odata.type": "microsoft.graph.outlookGeoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double",
      "accuracy": "Double",
      "altitudeAccuracy": "Double"
    },
    "locationUri": "Location Uri value",
    "locationType": "String",
    "uniqueId": "Unique Id value",
    "uniqueIdType": "String"
  },
  "customerNotes": "Customer Notes value",
  "serviceId": "Service Id value",
  "serviceName": "Service Name value",
  "start": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "Date Time value",
    "timeZone": "Time Zone value"
  },
  "end": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "duration": "-PT0.9940994S",
  "preBuffer": "-PT36.7327427S",
  "postBuffer": "PT3M21.6931326S",
  "serviceLocation": {
    "@odata.type": "microsoft.graph.location"
  },
  "priceType": "String",
  "price": "Double",
  "serviceNotes": "Service Notes value",
  "reminders": [
    {
      "@odata.type": "microsoft.graph.bookingReminder",
      "offset": "-PT43.7329867S",
      "recipients": "String",
      "message": "Message value"
    }
  ],
  "optOutOfCustomerEmail": true,
  "staffMemberIds": [
    "Staff Member Ids value"
  ],
  "invoiceAmount": "Double",
  "invoiceDate": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "invoiceId": "Invoice Id value",
  "invoiceStatus": "String",
  "invoiceUrl": "https://example.com/invoiceUrl/"
}
```

