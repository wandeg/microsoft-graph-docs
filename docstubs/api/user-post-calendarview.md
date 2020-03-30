---
title: "Add calendarView"
description: "Add calendarView by posting to the calendarView collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add calendarView

Namespace: microsoft.graph

Add calendarView by posting to the calendarView collection.

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
POST /me/calendarView/$ref
POST /users/{usersId}/calendarView/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [event](../resources/event.md) object.

The following table shows the properties that are required when you create the [event](../resources/event.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|changeKey|String| Inherited from [outlookItem](../resources/outlookitem.md)|
|categories|String collection| Inherited from [outlookItem](../resources/outlookitem.md)|
|transactionId|String||
|originalStartTimeZone|String||
|originalEndTimeZone|String||
|responseStatus|[responseStatus](../resources/responsestatus.md)||
|uid|String||
|reminderMinutesBeforeStart|Int32||
|isReminderOn|Boolean||
|hasAttachments|Boolean||
|subject|String||
|body|[itemBody](../resources/itembody.md)||
|bodyPreview|String||
|importance|Enumeration| Possible values are: `low`, `normal`, `high`.|
|sensitivity|Enumeration| Possible values are: `normal`, `personal`, `private`, `confidential`.|
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|originalStart|DateTimeOffset||
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|location|[location](../resources/location.md)||
|locations|[location](../resources/location.md) collection||
|isAllDay|Boolean||
|isCancelled|Boolean||
|isOrganizer|Boolean||
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)||
|responseRequested|Boolean||
|seriesMasterId|String||
|showAs|Enumeration| Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|type|Enumeration| Possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.|
|attendees|[attendee](../resources/attendee.md) collection||
|organizer|[recipient](../resources/recipient.md)||
|webLink|String||
|onlineMeetingUrl|String||
|isOnlineMeeting|Boolean||
|onlineMeetingProvider|Enumeration| Possible values are: `unknown`, `skypeForBusiness`, `skypeForConsumer`, `teamsForBusiness`.|
|onlineMeeting|[onlineMeetingInfo](../resources/onlinemeetinginfo.md)||
|allowNewTimeProposals|Boolean||
|isDraft|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [event](../resources/event.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_event_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/calendarView
Content-type: application/json
Content-length: 4104

{
  "@odata.type": "#microsoft.graph.event",
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
    "time": "2017-01-01T00:02:31.947532+03:00"
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
  "originalStart": "2016-12-31T23:57:17.99583+03:00",
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4276

{
  "@odata.type": "#microsoft.graph.event",
  "id": "d4e11b6e-1b6e-d4e1-6e1b-e1d46e1be1d4",
  "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
  "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
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
    "time": "2017-01-01T00:02:31.947532+03:00"
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
  "originalStart": "2016-12-31T23:57:17.99583+03:00",
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
```

