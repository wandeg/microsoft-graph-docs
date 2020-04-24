---
title: "Create calendarView"
description: "Create a new calendarView object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create calendarView

Namespace: microsoft.graph

Create a new calendarView object.

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
POST /me/calendarView
POST /users/{usersId}/calendarView
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [event](../resources/event.md) object.

The following table shows the properties that are required when you create the [event](../resources/event.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|changeKey|String|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|categories|String collection|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|transactionId|String|**TODO: Add Description**|
|originalStartTimeZone|String|**TODO: Add Description**|
|originalEndTimeZone|String|**TODO: Add Description**|
|responseStatus|[responseStatus](../resources/responsestatus.md)|**TODO: Add Description**|
|uid|String|**TODO: Add Description**|
|reminderMinutesBeforeStart|Int32|**TODO: Add Description**|
|isReminderOn|Boolean|**TODO: Add Description**|
|hasAttachments|Boolean|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|
|body|[itemBody](../resources/itembody.md)|**TODO: Add Description**|
|bodyPreview|String|**TODO: Add Description**|
|importance|importance|**TODO: Add Description**. Possible values are: `low`, `normal`, `high`.|
|sensitivity|sensitivity|**TODO: Add Description**. Possible values are: `normal`, `personal`, `private`, `confidential`.|
|start|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|originalStart|DateTimeOffset|**TODO: Add Description**|
|end|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|location|[location](../resources/location.md)|**TODO: Add Description**|
|locations|[location](../resources/location.md) collection|**TODO: Add Description**|
|isAllDay|Boolean|**TODO: Add Description**|
|isCancelled|Boolean|**TODO: Add Description**|
|isOrganizer|Boolean|**TODO: Add Description**|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|**TODO: Add Description**|
|responseRequested|Boolean|**TODO: Add Description**|
|seriesMasterId|String|**TODO: Add Description**|
|showAs|freeBusyStatus|**TODO: Add Description**. Possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|type|eventType|**TODO: Add Description**. Possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.|
|attendees|[attendee](../resources/attendee.md) collection|**TODO: Add Description**|
|organizer|[recipient](../resources/recipient.md)|**TODO: Add Description**|
|webLink|String|**TODO: Add Description**|
|onlineMeetingUrl|String|**TODO: Add Description**|
|isOnlineMeeting|Boolean|**TODO: Add Description**|
|onlineMeetingProvider|onlineMeetingProviderType|**TODO: Add Description**. Possible values are: `unknown`, `skypeForBusiness`, `skypeForConsumer`, `teamsForBusiness`.|
|onlineMeeting|[onlineMeetingInfo](../resources/onlinemeetinginfo.md)|**TODO: Add Description**|
|allowNewTimeProposals|Boolean|**TODO: Add Description**|
|isDraft|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [event](../resources/event.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_event_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/calendarView
Content-Type: application/json
Content-length: 4107

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
    "time": "2016-12-31T23:57:17.7513593+03:00"
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
  "originalStart": "2017-01-01T00:01:39.4679949+03:00",
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.event",
  "id": "2fa56ea9-6ea9-2fa5-a96e-a52fa96ea52f",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
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
    "time": "2016-12-31T23:57:17.7513593+03:00"
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
  "originalStart": "2017-01-01T00:01:39.4679949+03:00",
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

