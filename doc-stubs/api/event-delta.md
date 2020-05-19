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
|Authorization|Bearer {token}. Required.|

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
GET https://graph.microsoft.com/v1.0/me/events/delta
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
      "id": "String (identifier)",
      "createdDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)",
      "changeKey": "String",
      "categories": [
        "String"
      ],
      "originalStartTimeZone": "String",
      "originalEndTimeZone": "String",
      "responseStatus": {
        "@odata.type": "microsoft.graph.responseStatus"
      },
      "iCalUId": "String",
      "reminderMinutesBeforeStart": "Integer",
      "isReminderOn": "Boolean",
      "hasAttachments": "Boolean",
      "subject": "String",
      "body": {
        "@odata.type": "microsoft.graph.itemBody"
      },
      "bodyPreview": "String",
      "importance": "String",
      "sensitivity": "String",
      "start": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "originalStart": "String (timestamp)",
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
      "isAllDay": "Boolean",
      "isCancelled": "Boolean",
      "isOrganizer": "Boolean",
      "recurrence": {
        "@odata.type": "microsoft.graph.patternedRecurrence"
      },
      "responseRequested": "Boolean",
      "seriesMasterId": "String",
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
      "webLink": "String",
      "onlineMeetingUrl": "String",
      "isOnlineMeeting": "Boolean",
      "onlineMeetingProvider": "String",
      "onlineMeeting": {
        "@odata.type": "microsoft.graph.onlineMeetingInfo"
      },
      "allowNewTimeProposals": "Boolean"
    }
  ]
}
```

