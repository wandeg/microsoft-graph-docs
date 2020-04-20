---
title: "Get calendarPermission"
description: "Read properties and relationships of a calendarPermission object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get calendarPermission

Namespace: microsoft.graph

Read properties and relationships of a [calendarPermission](../resources/calendarpermission.md) object.

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
GET /invitations/{invitationsId}/invitedUser/messages/{messageId}/event/calendar/calendarPermissions/{calendarPermissionId}
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
If successful, this method returns a `200 OK` response code and a [calendarPermission](../resources/calendarpermission.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_calendarpermission"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/messages/{messageId}/event/calendar/calendarPermissions/{calendarPermissionId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarPermission"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.calendarPermission",
    "id": "b46d6294-6294-b46d-9462-6db494626db4",
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
}
```

