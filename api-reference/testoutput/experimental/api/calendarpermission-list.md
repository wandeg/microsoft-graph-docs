---
title: "List calendarPermissions"
description: "List properties and relationships of the calendarPermission objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List calendarPermissions

Namespace: microsoft.graph

List properties and relationships of the [calendarPermission](../resources/calendarpermission.md) objects.

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
GET /me/messages/{messageId}/event/calendar/calendarPermissions
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [calendarPermission](../resources/calendarpermission.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_calendarpermission"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/messages/{messageId}/event/calendar/calendarPermissions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.calendarpermission)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 451

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.calendarPermission",
      "id": "0445712f-712f-0445-2f71-45042f714504",
      "emailAddress": {
        "@odata.type": "microsoft.graph.emailAddress",
        "name": "Name value",
        "address": "Address value"
      },
      "isRemovable": true,
      "isInsideOrganization": true,
      "role": "String",
      "allowedRoles": [
        "String"
      ]
    }
  ]
}
```

