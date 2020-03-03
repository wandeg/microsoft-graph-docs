---
title: "cancel"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# cancel



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
POST /me/events/{eventId}/cancel
POST /me/calendarView/{eventId}/cancel
POST /me/messages/{messageId}/event/cancel
POST /users/{usersId}/events/{eventId}/cancel
POST /groups/{groupsId}/events/{eventId}/cancel
POST /users/{usersId}/calendarView/{eventId}/cancel
POST /groups/{groupsId}/calendarView/{eventId}/cancel
POST /me/joinedGroups/{groupId}/events/{eventId}/cancel
POST /me/joinedGroups/{groupId}/calendarView/{eventId}/cancel
POST /me/messages/{messageId}/event/instances/{eventId}/cancel
POST /me/messages/{messageId}/event/calendar/events/{eventId}/cancel
POST /me/messages/{messageId}/microsoft.graph.eventMessage/event/cancel
POST /me/messages/{messageId}/event/calendar/calendarView/{eventId}/cancel
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
|Comment|String||



## Response
If successful, this action returns a `204 No Content` response code.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "event_cancel"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/me/events/{eventId}/cancel

Content-type: application/json
Content-length: 34

{
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

