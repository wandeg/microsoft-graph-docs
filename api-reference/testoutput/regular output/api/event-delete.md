---
title: "Delete event"
description: "Deletes a event."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Delete event

Namespace: microsoft.graph

Deletes a [event](../resources/event.md).

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
DELETE /me/events/{eventId}
DELETE /me/calendarView/{eventId}
DELETE /users/{usersId}/events/{eventId}
DELETE /groups/{groupsId}/events/{eventId}
DELETE /users/{usersId}/calendarView/{eventId}
DELETE /groups/{groupsId}/calendarView/{eventId}
DELETE /me/joinedTeams/{groupId}/events/{eventId}
DELETE /me/joinedTeams/{groupId}/calendarView/{eventId}
DELETE /me/messages/{messageId}/microsoft.graph.eventMessage/event
DELETE /me/messages/{messageId}/microsoft.graph.eventMessage/event/instances/{eventId}
DELETE /me/messages/{messageId}/microsoft.graph.eventMessage/event/calendar/events/{eventId}
DELETE /me/messages/{messageId}/microsoft.graph.eventMessage/event/calendar/calendarView/{eventId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "delete_event"
}
-->
``` http
DELETE https://graph.microsoft.com/localtest/me/events/{eventId}
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

