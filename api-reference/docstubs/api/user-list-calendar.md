---
title: "List calendar"
description: "Get the calendars from the calendar navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List calendar

Namespace: microsoft.graph

Get the calendars from the calendar navigation property.

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
If successful, this method returns a `200 OK` response code and a collection of [calendar](../resources/calendar.md) objects in the response body.

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
  "@odata.type": "collection(microsoft.graph.calendar)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.calendar",
      "id": "2174eb44-eb44-2174-44eb-742144eb7421",
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
      "calendarGroupId": "Calendar Group Id value",
      "allowedOnlineMeetingProviders": [
        "String"
      ],
      "defaultOnlineMeetingProvider": "String",
      "isTallyingResponses": true,
      "isRemovable": true
    }
  ]
}
```

