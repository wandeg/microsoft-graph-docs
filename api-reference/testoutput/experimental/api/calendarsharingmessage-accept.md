---
title: "accept"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# accept

Namespace: microsoft.graph



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
POST ** Entity URI for microsoft.graph.calendarSharingMessage not found/accept
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [calendar](../resources/calendar.md) in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "calendarsharingmessage_accept"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.calendarSharingMessage not found/accept
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 658

{
  "value": {
    "@odata.type": "#microsoft.graph.calendar",
    "id": "00585ef7-5ef7-0058-f75e-5800f75e5800",
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
      "@odata.type": "microsoft.graph.emailAddress"
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

