---
title: "List services"
description: "Get the bookingServices from the services navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List services

Namespace: microsoft.graph

Get the bookingServices from the services navigation property.

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
GET /bookingBusinesses/{bookingBusinessesId}/services
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [bookingService](../resources/bookingservice.md) objects in the response body.

## Examples

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
Content-Length: 2100

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bookingService",
      "id": "73924ea1-4ea1-7392-a14e-9273a14e9273",
      "displayName": "Display Name value",
      "defaultDuration": "PT3M29.2405346S",
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
          "offset": "-PT48.1154137S",
          "recipients": "String",
          "message": "Message value"
        }
      ],
      "description": "Description value",
      "isHiddenFromCustomers": true,
      "notes": "Notes value",
      "preBuffer": "-PT2M36.5986877S",
      "postBuffer": "PT1M50.7470612S",
      "schedulingPolicy": {
        "@odata.type": "microsoft.graph.bookingSchedulingPolicy",
        "timeSlotInterval": "-PT2M6.5040939S",
        "minimumLeadTime": "PT1M46.8466139S",
        "maximumAdvance": "-PT34.7669238S",
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

