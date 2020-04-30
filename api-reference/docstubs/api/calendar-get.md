---
title: "Get calendar"
description: "Read the properties and relationships of a calendar object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get calendar

Namespace: microsoft.graph

Read the properties and relationships of a [calendar](../resources/calendar.md) object.

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
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

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
**Note:** The response object shown here might be shortened for readability.
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
    "id": "f7e9cc69-cc69-f7e9-69cc-e9f769cce9f7",
    "name": "String",
    "color": "String",
    "hexColor": "String",
    "isDefaultCalendar": "Boolean",
    "changeKey": "String",
    "canShare": "Boolean",
    "canViewPrivateItems": "Boolean",
    "isShared": "Boolean",
    "isSharedWithMe": "Boolean",
    "canEdit": "Boolean",
    "owner": {
      "@odata.type": "microsoft.graph.emailAddress"
    },
    "calendarGroupId": "String",
    "allowedOnlineMeetingProviders": [
      "String"
    ],
    "defaultOnlineMeetingProvider": "String",
    "isTallyingResponses": "Boolean",
    "isRemovable": "Boolean"
  }
}
```

