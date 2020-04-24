---
title: "List calendarView"
description: "Get the bookingAppointments from the calendarView navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List calendarView

Namespace: microsoft.graph

Get the bookingAppointments from the calendarView navigation property.

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
GET /bookingBusinesses/{bookingBusinessesId}/calendarView
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [bookingAppointment](../resources/bookingappointment.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}
-->
``` http
GET https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}/calendarView
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.bookingappointment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

