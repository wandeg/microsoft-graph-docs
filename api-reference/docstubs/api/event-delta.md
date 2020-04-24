---
title: "event: delta"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# delta

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /me/events/delta
GET /me/calendarView/delta
GET /users/{usersId}/events/delta
GET /groups/{groupsId}/events/delta
GET /users/{usersId}/calendarView/delta
GET /groups/{groupsId}/calendarView/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [event](../resources/event.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "event_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/events/delta
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.event)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
        "@odata.type": "microsoft.graph.responseStatus"
      },
      "uid": "Uid value",
      "reminderMinutesBeforeStart": 10,
      "isReminderOn": true,
      "hasAttachments": true,
      "subject": "Subject value",
      "body": {
        "@odata.type": "microsoft.graph.itemBody"
      },
      "bodyPreview": "Body Preview value",
      "importance": "String",
      "sensitivity": "String",
      "start": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "originalStart": "2017-01-01T00:01:39.4679949+03:00",
      "end": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "location": {
        "@odata.type": "microsoft.graph.location"
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
        "@odata.type": "microsoft.graph.patternedRecurrence"
      },
      "responseRequested": true,
      "seriesMasterId": "Series Master Id value",
      "showAs": "String",
      "type": "String",
      "attendees": [
        {
          "@odata.type": "microsoft.graph.attendee"
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
        "@odata.type": "microsoft.graph.onlineMeetingInfo"
      },
      "allowNewTimeProposals": true,
      "isDraft": true
    }
  ]
}
```

