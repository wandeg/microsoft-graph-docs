---
title: "List calendars"
description: "Get the calendars from the calendars navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List calendars

Get the calendars from the calendars navigation property.

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
GET /me/calendarGroups/{calendarGroupId}/calendars
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [calendar](../resources/calendar.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_calendar"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/me/calendarGroups/{calendarGroupId}/calendars
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.calendar)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 751

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.calendar",
      "id": "cfde7b0b-7b0b-cfde-0b7b-decf0b7bdecf",
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
  ]
}
```

