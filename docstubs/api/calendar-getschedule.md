---
title: "calendar: getSchedule"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getSchedule

Namespace: microsoft.graph



## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions. **|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/calendar/getSchedule
POST /users/{usersId}/calendar/getSchedule
POST /me/calendars/{calendarId}/getSchedule
POST /groups/{groupsId}/calendar/getSchedule
POST /me/joinedGroups/{groupId}/calendar/getSchedule
POST /me/messages/{messageId}/event/calendar/getSchedule
POST /users/{usersId}/calendars/{calendarId}/getSchedule
POST /me/calendarGroups/{calendarGroupId}/calendars/{calendarId}/getSchedule
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|Schedules|String collection||
|EndTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|StartTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|AvailabilityViewInterval|Int32||



## Response
If successful, this action returns a `200 OK` response code and a [scheduleInformation](../resources/scheduleinformation.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "calendar_getschedule"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/calendar/getSchedule

Content-type: application/json
Content-length: 240

{
  "Schedules": [
    "Schedules value"
  ],
  "EndTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "StartTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "AvailabilityViewInterval": 8
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.scheduleinformation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 97

{
  "value": [
    {
      "@odata.type": "microsoft.graph.scheduleInformation"
    }
  ]
}
```

