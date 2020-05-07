---
title: "Get bookingAppointment"
description: "Read the properties and relationships of a bookingAppointment object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get bookingAppointment

Namespace: microsoft.graph

Read the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object.

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
GET /bookingBusinesses/{bookingBusinessesId}/appointments/{bookingAppointmentId}
GET /bookingBusinesses/{bookingBusinessesId}/calendarView/{bookingAppointmentId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [bookingAppointment](../resources/bookingappointment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}
-->
``` http
GET https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}/appointments/{bookingAppointmentId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
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
}
```

