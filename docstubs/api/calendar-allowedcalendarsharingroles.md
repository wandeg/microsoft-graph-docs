---
title: "allowedCalendarSharingRoles"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# allowedCalendarSharingRoles

Namespace: microsoft.graph



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
GET /me/calendar/allowedCalendarSharingRoles
GET /users/{usersId}/calendar/allowedCalendarSharingRoles
GET /me/calendars/{calendarId}/allowedCalendarSharingRoles
GET /groups/{groupsId}/calendar/allowedCalendarSharingRoles
GET /me/joinedGroups/{groupId}/calendar/allowedCalendarSharingRoles
GET /me/messages/{messageId}/event/calendar/allowedCalendarSharingRoles
GET /users/{usersId}/calendars/{calendarId}/allowedCalendarSharingRoles
GET /me/calendarGroups/{calendarGroupId}/calendars/{calendarId}/allowedCalendarSharingRoles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|User|String||



## Response
If successful, this function returns a `200 OK` response code and a Enumeration collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "calendar_allowedcalendarsharingroles"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/calendar/allowedCalendarSharingRoles(User='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.calendarroletype)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 37

{
  "value": [
    "String"
  ]
}
```

