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
|Name|Description|
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
GET https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}/services
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
Content-Length: 2101

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bookingService",
      "id": "22196f7c-6f7c-2219-7c6f-19227c6f1922",
      "displayName": "Display Name value",
      "defaultDuration": "-PT47.0007377S",
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
          "offset": "-PT2M48.5182876S",
          "recipients": "String",
          "message": "Message value"
        }
      ],
      "description": "Description value",
      "isHiddenFromCustomers": true,
      "notes": "Notes value",
      "preBuffer": "PT1M52.4181917S",
      "postBuffer": "PT1M14.7348885S",
      "schedulingPolicy": {
        "@odata.type": "microsoft.graph.bookingSchedulingPolicy",
        "timeSlotInterval": "PT1M16.5548848S",
        "minimumLeadTime": "PT3M16.1082793S",
        "maximumAdvance": "PT2M55.4131499S",
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

