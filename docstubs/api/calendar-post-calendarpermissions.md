---
title: "Add calendarPermissions"
description: "Add calendarPermissions by posting to the calendarPermissions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add calendarPermissions

Namespace: microsoft.graph

Add calendarPermissions by posting to the calendarPermissions collection.

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
POST /me/messages/{messageId}/event/calendar/calendarPermissions/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [calendarPermission](../resources/calendarpermission.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_calendarpermission_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/messages/{messageId}/event/calendar/calendarPermissions
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
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarpermission"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 366

{
  "@odata.type": "#microsoft.graph.calendarPermission",
  "id": "5ad564aa-64aa-5ad5-aa64-d55aaa64d55a",
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

