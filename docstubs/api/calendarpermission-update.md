---
title: "Update calendarPermission"
description: "Update the properties of a calendarPermission object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update calendarPermission

Namespace: microsoft.graph

Update the properties of a [calendarPermission](../resources/calendarpermission.md) object.

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
PATCH /me/messages/{messageId}/microsoft.graph.eventMessage/event/calendar/calendarPermissions/{calendarPermissionId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [calendarPermission](../resources/calendarpermission.md) object.

The following table shows the properties that are required when you create the [calendarPermission](../resources/calendarpermission.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|emailAddress|[emailAddress](../resources/emailaddress.md)||
|isRemovable|Boolean||
|isInsideOrganization|Boolean||
|role|Enumeration| Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|
|allowedRoles|Enumeration collection| Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [calendarPermission](../resources/calendarpermission.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_calendarpermission"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/me/messages/{messageId}/microsoft.graph.eventMessage/event/calendar/calendarPermissions/{calendarPermissionId}
Content-type: application/json
Content-length: 317

{
  "@odata.type": "#microsoft.graph.calendarPermission",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 366

{
  "@odata.type": "#microsoft.graph.calendarPermission",
  "id": "dcf73126-3126-dcf7-2631-f7dc2631f7dc",
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
```

