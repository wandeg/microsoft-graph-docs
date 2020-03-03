---
title: "Add appointments"
description: "Add appointments by posting to the appointments collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add appointments

Add appointments by posting to the appointments collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /bookingBusinesses/{bookingBusinessesId}/appointments/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the bookingAppointment object.

The following table shows the properties that are required when you create the bookingAppointment.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|selfServiceAppointmentId|String||
|customerId|String|The id of the booking customer associated with this appointment.
If CustomerId is not specified when an appointment is created then a new customer is created based on the appointment customer information. Once set, the customerId should be considered immutable.|
|customerName|String||
|customerEmailAddress|String||
|customerPhone|String||
|customerLocation|[location](../resources/location.md)||
|customerNotes|String|Notes from the customer associated with this appointment.
The value of this property is only available when reading an individual booking appointment by id. Its value can only be set when creating a new appointment with a new customer, ie, without specifying a CustomerId. After that, the property is computed from the customer represented by CustomerId.|
|serviceId|String|The id of the booking service associated with this appointment.|
|serviceName|String|The name of the booking service associated with this appointment.
This property is optional when creating a new appointment. If not specified, it is computed from the service associated with the appointment by the service id.|
|start|[dateTimeTimeZone](../resources/dateTimeTimeZone.md)||
|end|[dateTimeTimeZone](../resources/dateTimeTimeZone.md)||
|duration|Duration||
|preBuffer|Duration||
|postBuffer|Duration||
|serviceLocation|[location](../resources/location.md)||
|priceType|Enumeration|. Possible values are: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`.|
|price|Double||
|serviceNotes|String|The value of this property is only available when reading an individual booking appointment by id.|
|reminders|[bookingReminder](../resources/bookingReminder.md) collection|The value of this property is only available when reading an individual booking appointment by id.|
|optOutOfCustomerEmail|Boolean||
|staffMemberIds|String collection||
|invoiceAmount|Double||
|invoiceDate|[dateTimeTimeZone](../resources/dateTimeTimeZone.md)||
|invoiceId|String||
|invoiceStatus|Enumeration|. Possible values are: `draft`, `reviewing`, `open`, `canceled`, `paid`, `corrective`.|
|invoiceUrl|String||



## Response
If successful, this method returns a `201 Created` response code and a [bookingAppointment](../resources/bookingappointment.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_bookingappointment_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/bookingBusinesses/{bookingBusinessesId}/appointments
Content-type: application/json
Content-length: 2349

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
  "duration": "PT3M27.7161587S",
  "preBuffer": "PT3M13.876457S",
  "postBuffer": "-PT3M7.6941789S",
  "serviceLocation": {
    "@odata.type": "microsoft.graph.location"
  },
  "priceType": "String",
  "price": "Double",
  "serviceNotes": "Service Notes value",
  "reminders": [
    {
      "@odata.type": "microsoft.graph.bookingReminder",
      "offset": "PT29.4091216S",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingappointment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2398

{
  "@odata.type": "#microsoft.graph.bookingAppointment",
  "id": "bcb5ac85-ac85-bcb5-85ac-b5bc85acb5bc",
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
  "duration": "PT3M27.7161587S",
  "preBuffer": "PT3M13.876457S",
  "postBuffer": "-PT3M7.6941789S",
  "serviceLocation": {
    "@odata.type": "microsoft.graph.location"
  },
  "priceType": "String",
  "price": "Double",
  "serviceNotes": "Service Notes value",
  "reminders": [
    {
      "@odata.type": "microsoft.graph.bookingReminder",
      "offset": "PT29.4091216S",
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

