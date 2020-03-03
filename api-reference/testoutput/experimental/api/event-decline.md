---
title: "decline"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# decline

Namespace: microsoft.graph



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
POST /me/events/{eventId}/decline
POST /me/calendarView/{eventId}/decline
POST /me/messages/{messageId}/event/decline
POST /users/{usersId}/events/{eventId}/decline
POST /groups/{groupsId}/events/{eventId}/decline
POST /users/{usersId}/calendarView/{eventId}/decline
POST /groups/{groupsId}/calendarView/{eventId}/decline
POST /me/joinedGroups/{groupId}/events/{eventId}/decline
POST /me/joinedGroups/{groupId}/calendarView/{eventId}/decline
POST /me/messages/{messageId}/event/instances/{eventId}/decline
POST /me/messages/{messageId}/event/calendar/events/{eventId}/decline
POST /me/messages/{messageId}/microsoft.graph.eventMessage/event/decline
POST /me/messages/{messageId}/event/calendar/calendarView/{eventId}/decline
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|ProposedNewTime|[timeSlot](../resources/timeslot.md)||
|SendResponse|Boolean||
|Comment|String||



## Response
If successful, this action returns a `204 No Content` response code.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "event_decline"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/events/{eventId}/decline

Content-type: application/json
Content-length: 136

{
  "ProposedNewTime": {
    "@odata.type": "microsoft.graph.timeSlot"
  },
  "SendResponse": true,
  "Comment": "Comment value"
}
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

