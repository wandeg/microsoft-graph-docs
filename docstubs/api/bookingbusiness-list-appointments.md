---
title: "List appointments"
description: "Get the bookingAppointments from the appointments navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List appointments

Namespace: microsoft.graph

Get the bookingAppointments from the appointments navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /bookingBusinesses/{bookingBusinessesId}/appointments
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [bookingAppointment](../resources/bookingappointment.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}
-->
``` http
GET https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}/appointments
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.bookingappointment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2727

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bookingAppointment",
      "id": "a48fabdf-abdf-a48f-dfab-8fa4dfab8fa4",
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
      "duration": "-PT2M12.8464123S",
      "preBuffer": "PT2M27.2286073S",
      "postBuffer": "-PT1M59.4076097S",
      "serviceLocation": {
        "@odata.type": "microsoft.graph.location"
      },
      "priceType": "String",
      "price": "Double",
      "serviceNotes": "Service Notes value",
      "reminders": [
        {
          "@odata.type": "microsoft.graph.bookingReminder",
          "offset": "-PT56.3619857S",
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

