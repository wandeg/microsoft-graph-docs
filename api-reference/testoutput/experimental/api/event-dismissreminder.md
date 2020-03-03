---
title: "dismissReminder"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# dismissReminder



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
POST /me/events/{eventId}/dismissReminder
POST /me/calendarView/{eventId}/dismissReminder
POST /me/messages/{messageId}/event/dismissReminder
POST /users/{usersId}/events/{eventId}/dismissReminder
POST /groups/{groupsId}/events/{eventId}/dismissReminder
POST /users/{usersId}/calendarView/{eventId}/dismissReminder
POST /groups/{groupsId}/calendarView/{eventId}/dismissReminder
POST /me/joinedGroups/{groupId}/events/{eventId}/dismissReminder
POST /me/joinedGroups/{groupId}/calendarView/{eventId}/dismissReminder
POST /me/messages/{messageId}/event/instances/{eventId}/dismissReminder
POST /me/messages/{messageId}/event/calendar/events/{eventId}/dismissReminder
POST /me/messages/{messageId}/microsoft.graph.eventMessage/event/dismissReminder
POST /me/messages/{messageId}/event/calendar/calendarView/{eventId}/dismissReminder
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `204 No Content` response code.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "event_dismissreminder"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/me/events/{eventId}/dismissReminder
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

