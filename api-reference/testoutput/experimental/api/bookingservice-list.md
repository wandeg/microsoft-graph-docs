---
title: "List bookingServices"
description: "List properties and relationships of the bookingService objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List bookingServices

Namespace: microsoft.graph

List properties and relationships of the [bookingService](../resources/bookingservice.md) objects.

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
GET /bookingBusinesses/{bookingBusinessesId}/services
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [bookingService](../resources/bookingservice.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_bookingservice"
}
-->
``` http
GET https://graph.microsoft.com/localtest/bookingBusinesses/{bookingBusinessesId}/services
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.bookingservice)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2094

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bookingService",
      "id": "dcfd9872-9872-dcfd-7298-fddc7298fddc",
      "displayName": "Display Name value",
      "defaultDuration": "PT2M30.8894523S",
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
          "offset": "-PT2M15.3589096S",
          "recipients": "String",
          "message": "Message value"
        }
      ],
      "description": "Description value",
      "isHiddenFromCustomers": true,
      "notes": "Notes value",
      "preBuffer": "-PT27.6468082S",
      "postBuffer": "-PT49.745402S",
      "schedulingPolicy": {
        "@odata.type": "microsoft.graph.bookingSchedulingPolicy",
        "timeSlotInterval": "PT24.7084489S",
        "minimumLeadTime": "PT46.1171008S",
        "maximumAdvance": "-PT29.5884928S",
        "sendConfirmationsToOwner": true,
        "allowStaffSelection": true
      },
      "staffMemberIds": [
        "Staff Member Ids value"
      ]
    }
  ]
}
```

