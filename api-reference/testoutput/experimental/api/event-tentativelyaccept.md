---
title: "tentativelyAccept"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# tentativelyAccept

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
POST /me/events/{eventId}/tentativelyAccept
POST /me/calendarView/{eventId}/tentativelyAccept
POST /me/messages/{messageId}/event/tentativelyAccept
POST /users/{usersId}/events/{eventId}/tentativelyAccept
POST /groups/{groupsId}/events/{eventId}/tentativelyAccept
POST /users/{usersId}/calendarView/{eventId}/tentativelyAccept
POST /groups/{groupsId}/calendarView/{eventId}/tentativelyAccept
POST /me/joinedGroups/{groupId}/events/{eventId}/tentativelyAccept
POST /me/joinedGroups/{groupId}/calendarView/{eventId}/tentativelyAccept
POST /me/messages/{messageId}/event/instances/{eventId}/tentativelyAccept
POST /me/messages/{messageId}/event/calendar/events/{eventId}/tentativelyAccept
POST /me/messages/{messageId}/microsoft.graph.eventMessage/event/tentativelyAccept
POST /me/messages/{messageId}/event/calendar/calendarView/{eventId}/tentativelyAccept
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
  "name": "event_tentativelyaccept"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/events/{eventId}/tentativelyAccept

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

