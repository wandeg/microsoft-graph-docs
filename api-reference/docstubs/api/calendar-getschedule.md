---
title: "calendar: getSchedule"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getSchedule

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
POST /me/calendar/getSchedule
POST /users/{usersId}/calendar/getSchedule
POST /me/calendars/{calendarId}/getSchedule
POST /groups/{groupsId}/calendar/getSchedule
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|Schedules|String collection|**TODO: Add Description**|
|EndTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|StartTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|AvailabilityViewInterval|Int32|**TODO: Add Description**|



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

Content-Type: application/json
Content-length: 239

{
  "Schedules": [
    "String"
  ],
  "EndTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "StartTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "AvailabilityViewInterval": "Integer"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.scheduleinformation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "microsoft.graph.scheduleInformation"
    }
  ]
}
```

