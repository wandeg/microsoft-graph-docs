---
title: "calendar: allowedCalendarSharingRoles"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# allowedCalendarSharingRoles

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
GET /me/calendar/allowedCalendarSharingRoles
GET /users/{usersId}/calendar/allowedCalendarSharingRoles
GET /me/calendars/{calendarId}/allowedCalendarSharingRoles
GET /groups/{groupsId}/calendar/allowedCalendarSharingRoles
GET /users/{usersId}/calendars/{calendarId}/allowedCalendarSharingRoles
GET /invitations/{invitationsId}/invitedUser/calendar/allowedCalendarSharingRoles
GET /invitations/{invitationsId}/invitedUser/calendars/{calendarId}/allowedCalendarSharingRoles
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/calendar/allowedCalendarSharingRoles
GET /invitations/{invitationsId}/invitedUser/messages/{messageId}/event/calendar/allowedCalendarSharingRoles
GET /invitations/{invitationsId}/invitedUser/calendarGroups/{calendarGroupId}/calendars/{calendarId}/allowedCalendarSharingRoles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|User|String|**TODO: Add Description**|



## Response
If successful, this function returns a `200 OK` response code and a calendarRoleType collection, which can contain the following values: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom` in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "calendar_allowedcalendarsharingroles"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/calendar/allowedCalendarSharingRoles(User='parameterValue')
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.calendarroletype)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    "String"
  ]
}
```

