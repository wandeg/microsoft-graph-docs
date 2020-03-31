---
title: "Get bookingService"
description: "Read properties and relationships of the bookingService object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get bookingService

Namespace: microsoft.graph

Read properties and relationships of the [bookingService](../resources/bookingservice.md) object.

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
GET /bookingBusinesses/{bookingBusinessesId}/services/{bookingServiceId}
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
If successful, this method returns a `200 OK` response code and [bookingService](../resources/bookingservice.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_bookingservice"
}
-->
``` http
GET https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}/services/{bookingServiceId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1976

{
  "value": {
    "@odata.type": "#microsoft.graph.bookingService",
    "id": "46c60140-0140-46c6-4001-c6464001c646",
    "displayName": "Display Name value",
    "defaultDuration": "-PT10.3545857S",
    "defaultLocation": {
      "@odata.type": "microsoft.graph.location",
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
    "defaultPrice": "Double",
    "defaultPriceType": "String",
    "defaultReminders": [
      {
        "@odata.type": "microsoft.graph.bookingReminder",
        "offset": "-PT1M18.3350919S",
        "recipients": "String",
        "message": "Message value"
      }
    ],
    "description": "Description value",
    "isHiddenFromCustomers": true,
    "notes": "Notes value",
    "preBuffer": "-PT1M47.5203165S",
    "postBuffer": "-PT23.3579744S",
    "schedulingPolicy": {
      "@odata.type": "microsoft.graph.bookingSchedulingPolicy",
      "timeSlotInterval": "-PT3M1.5903122S",
      "minimumLeadTime": "PT3M18.5938901S",
      "maximumAdvance": "-PT2M40.3787358S",
      "sendConfirmationsToOwner": true,
      "allowStaffSelection": true
    },
    "staffMemberIds": [
      "Staff Member Ids value"
    ]
  }
}
```

