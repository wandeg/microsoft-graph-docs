---
title: "forward"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# forward



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
POST /me/events/{eventId}/forward
POST /me/calendarView/{eventId}/forward
POST /me/messages/{messageId}/event/forward
POST /users/{usersId}/events/{eventId}/forward
POST /groups/{groupsId}/events/{eventId}/forward
POST /users/{usersId}/calendarView/{eventId}/forward
POST /groups/{groupsId}/calendarView/{eventId}/forward
POST /me/joinedGroups/{groupId}/events/{eventId}/forward
POST /me/joinedGroups/{groupId}/calendarView/{eventId}/forward
POST /me/messages/{messageId}/event/instances/{eventId}/forward
POST /me/messages/{messageId}/event/calendar/events/{eventId}/forward
POST /me/messages/{messageId}/microsoft.graph.eventMessage/event/forward
POST /me/messages/{messageId}/event/calendar/calendarView/{eventId}/forward
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
|ToRecipients|[recipient](../resources/recipient.md) collection||
|Comment|String||



## Response
If successful, this action returns a `204 No Content` response code.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "event_forward"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/me/events/{eventId}/forward

Content-type: application/json
Content-length: 125

{
  "ToRecipients": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
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

