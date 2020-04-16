---
title: "Get calendar"
description: "Read properties and relationships of a calendar object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get calendar

Namespace: microsoft.graph

Read properties and relationships of a [calendar](../resources/calendar.md) object.

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
GET /me/calendar
GET /users/{usersId}/calendar
GET /me/calendars/{calendarId}
GET /groups/{groupsId}/calendar
GET /me/joinedGroups/{groupId}/calendar
GET /me/messages/{messageId}/event/calendar
GET /users/{usersId}/calendars/{calendarId}
GET /me/calendarGroups/{calendarGroupId}/calendars/{calendarId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [calendar](../resources/calendar.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/calendar
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.calendar",
    "id": "414f6b47-6b47-414f-476b-4f41476b4f41",
    "name": "Name value",
    "color": "String",
    "hexColor": "Hex Color value",
    "isDefaultCalendar": true,
    "changeKey": "Change Key value",
    "canShare": true,
    "canViewPrivateItems": true,
    "isShared": true,
    "isSharedWithMe": true,
    "canEdit": true,
    "owner": {
      "@odata.type": "microsoft.graph.emailAddress",
      "address": "Address value"
    },
    "allowedOnlineMeetingProviders": [
      "String"
    ],
    "defaultOnlineMeetingProvider": "String",
    "isTallyingResponses": true,
    "isRemovable": true
  }
}
```

