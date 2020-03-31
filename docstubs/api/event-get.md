---
title: "Get event"
description: "Read properties and relationships of the event object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get event

Namespace: microsoft.graph

Read properties and relationships of the [event](../resources/event.md) object.

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
GET /me/events/{eventId}
GET /me/calendarView/{eventId}
GET /me/messages/{messageId}/event
GET /users/{usersId}/events/{eventId}
GET /groups/{groupsId}/events/{eventId}
GET /users/{usersId}/calendarView/{eventId}
GET /groups/{groupsId}/calendarView/{eventId}
GET /me/joinedGroups/{groupId}/events/{eventId}
GET /me/joinedGroups/{groupId}/calendarView/{eventId}
GET /me/messages/{messageId}/event/instances/{eventId}
GET /me/messages/{messageId}/event/calendar/events/{eventId}
GET /me/messages/{messageId}/microsoft.graph.eventMessage/event
GET /me/messages/{messageId}/event/calendar/calendarView/{eventId}
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
If successful, this method returns a `200 OK` response code and [event](../resources/event.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_event"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/events/{eventId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4584

{
  "value": {
    "@odata.type": "#microsoft.graph.event",
    "id": "9b9448e9-48e9-9b94-e948-949be948949b",
    "createdDateTime": "2016-12-31T23:57:50.7767122+03:00",
    "lastModifiedDateTime": "2017-01-01T00:01:52.9217945+03:00",
    "changeKey": "Change Key value",
    "categories": [
      "Categories value"
    ],
    "transactionId": "Transaction Id value",
    "originalStartTimeZone": "Original Start Time Zone value",
    "originalEndTimeZone": "Original End Time Zone value",
    "responseStatus": {
      "@odata.type": "microsoft.graph.responseStatus",
      "response": "String",
      "time": "2016-12-31T23:57:48.4426607+03:00"
    },
    "uid": "Uid value",
    "reminderMinutesBeforeStart": 10,
    "isReminderOn": true,
    "hasAttachments": true,
    "subject": "Subject value",
    "body": {
      "@odata.type": "microsoft.graph.itemBody",
      "contentType": "String",
      "content": "Content value"
    },
    "bodyPreview": "Body Preview value",
    "importance": "String",
    "sensitivity": "String",
    "start": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone",
      "dateTime": "Date Time value",
      "timeZone": "Time Zone value"
    },
    "originalStart": "2017-01-01T00:01:57.0830014+03:00",
    "end": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "location": {
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
    "locations": [
      {
        "@odata.type": "microsoft.graph.location"
      }
    ],
    "isAllDay": true,
    "isCancelled": true,
    "isOrganizer": true,
    "recurrence": {
      "@odata.type": "microsoft.graph.patternedRecurrence",
      "pattern": {
        "@odata.type": "microsoft.graph.recurrencePattern",
        "type": "String",
        "interval": 8,
        "month": 5,
        "dayOfMonth": 10,
        "daysOfWeek": [
          "String"
        ],
        "firstDayOfWeek": "String",
        "index": "String"
      },
      "range": {
        "@odata.type": "microsoft.graph.recurrenceRange",
        "type": "String",
        "startDate": "Date",
        "endDate": "Date",
        "recurrenceTimeZone": "Recurrence Time Zone value",
        "numberOfOccurrences": 3
      }
    },
    "responseRequested": true,
    "seriesMasterId": "Series Master Id value",
    "showAs": "String",
    "type": "String",
    "attendees": [
      {
        "@odata.type": "microsoft.graph.attendee",
        "emailAddress": {
          "@odata.type": "microsoft.graph.emailAddress",
          "name": "Name value",
          "address": "Address value"
        },
        "type": "String",
        "status": {
          "@odata.type": "microsoft.graph.responseStatus"
        },
        "proposedNewTime": {
          "@odata.type": "microsoft.graph.timeSlot"
        }
      }
    ],
    "organizer": {
      "@odata.type": "microsoft.graph.recipient"
    },
    "webLink": "Web Link value",
    "onlineMeetingUrl": "https://example.com/onlineMeetingUrl/",
    "isOnlineMeeting": true,
    "onlineMeetingProvider": "String",
    "onlineMeeting": {
      "@odata.type": "microsoft.graph.onlineMeetingInfo",
      "joinUrl": "https://example.com/joinUrl/",
      "conferenceId": "Conference Id value",
      "tollNumber": "Toll Number value",
      "tollFreeNumbers": [
        "Toll Free Numbers value"
      ],
      "quickDial": "Quick Dial value",
      "phones": [
        {
          "@odata.type": "microsoft.graph.phone",
          "type": "String",
          "number": "Number value"
        }
      ]
    },
    "allowNewTimeProposals": true,
    "isDraft": true
  }
}
```

