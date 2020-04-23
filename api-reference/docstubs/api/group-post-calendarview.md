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
POST /groups/{groupsId}/calendarView
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
|originalStartTimeZone|String|**TODO: Add Description**|
|originalEndTimeZone|String|**TODO: Add Description**|
|responseStatus|[responseStatus](../resources/responsestatus.md)|**TODO: Add Description**|
|iCalUId|String|**TODO: Add Description**|
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
POST https://graph.microsoft.com/beta/groups/{groupsId}/calendarView
Content-Type: application/json
Content-length: 3315

{
  "@odata.type": "#microsoft.graph.event",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "originalStartTimeZone": "Original Start Time Zone value",
  "originalEndTimeZone": "Original End Time Zone value",
  "responseStatus": {
    "@odata.type": "microsoft.graph.responseStatus",
    "response": "String",
    "time": "2016-12-31T23:57:03.4379316+03:00"
  },
  "iCalUId": "ICal UId value",
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
  "originalStart": "2017-01-01T00:03:22.4760242+03:00",
  "end": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "location": {
    "@odata.type": "microsoft.graph.location",
    "displayName": "Display Name value",
    "locationEmailAddress": "Location Email Address value",
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryOrRegion": "Country Or Region value",
      "postalCode": "Postal Code value"
    },
    "locationUri": "Location Uri value",
    "coordinates": {
      "@odata.type": "microsoft.graph.outlookGeoCoordinates",
      "latitude": "Double",
      "longitude": "Double",
      "accuracy": "Double",
      "altitude": "Double",
      "altitudeAccuracy": "Double"
    },
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
      }
    }
  ],
  "organizer": {
    "@odata.type": "microsoft.graph.recipient"
  },
  "webLink": "Web Link value",
  "onlineMeetingUrl": "https://example.com/onlineMeetingUrl/"
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
  "id": "95640543-0543-9564-4305-649543056495",
  "createdDateTime": "2017-01-01T00:02:24.9669049+03:00",
  "lastModifiedDateTime": "2017-01-01T00:02:46.687785+03:00",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "originalStartTimeZone": "Original Start Time Zone value",
  "originalEndTimeZone": "Original End Time Zone value",
  "responseStatus": {
    "@odata.type": "microsoft.graph.responseStatus",
    "response": "String",
    "time": "2016-12-31T23:57:03.4379316+03:00"
  },
  "iCalUId": "ICal UId value",
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
  "originalStart": "2017-01-01T00:03:22.4760242+03:00",
  "end": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "location": {
    "@odata.type": "microsoft.graph.location",
    "displayName": "Display Name value",
    "locationEmailAddress": "Location Email Address value",
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryOrRegion": "Country Or Region value",
      "postalCode": "Postal Code value"
    },
    "locationUri": "Location Uri value",
    "coordinates": {
      "@odata.type": "microsoft.graph.outlookGeoCoordinates",
      "latitude": "Double",
      "longitude": "Double",
      "accuracy": "Double",
      "altitude": "Double",
      "altitudeAccuracy": "Double"
    },
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
      }
    }
  ],
  "organizer": {
    "@odata.type": "microsoft.graph.recipient"
  },
  "webLink": "Web Link value",
  "onlineMeetingUrl": "https://example.com/onlineMeetingUrl/"
}
```

