---
title: "List calendar"
description: "Get the calendars from the calendar navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
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
GET /invitations/{invitationsId}/invitedUser/calendar/events/{eventId}/calendar
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
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/calendar/events/{eventId}/calendar
```

### Response
**Note:** The response object shown here might be shortened for readability.
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
      "id": "7f7bdf7f-df7f-7f7b-7fdf-7b7f7fdf7b7f",
      "name": "Name value",
      "color": "String",
      "changeKey": "Change Key value",
      "canShare": true,
      "canViewPrivateItems": true,
      "canEdit": true,
      "owner": {
        "@odata.type": "microsoft.graph.emailAddress",
        "address": "Address value"
      }
    }
  ]
}
```

