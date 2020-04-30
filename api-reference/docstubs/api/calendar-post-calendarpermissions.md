---
title: "Create calendarPermissions"
description: "Create a new calendarPermissions object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create calendarPermissions

Namespace: microsoft.graph

Create a new calendarPermissions object.

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
POST /users/{usersId}/messages/{messageId}/event/calendar/calendarPermissions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [calendarPermission](../resources/calendarpermission.md) object.

The following table shows the properties that are required when you create the [calendarPermission](../resources/calendarpermission.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|emailAddress|[emailAddress](../resources/emailaddress.md)|**TODO: Add Description**|
|isRemovable|Boolean|**TODO: Add Description**|
|isInsideOrganization|Boolean|**TODO: Add Description**|
|role|calendarRoleType|**TODO: Add Description**. Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|
|allowedRoles|calendarRoleType collection|**TODO: Add Description**. Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|



## Response
If successful, this method returns a `201 Created` response code and a [calendarPermission](../resources/calendarpermission.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_calendarpermission_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/messages/{messageId}/event/calendar/calendarPermissions
Content-Type: application/json
Content-length: 267

{
  "@odata.type": "#microsoft.graph.calendarPermission",
  "emailAddress": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "isRemovable": "Boolean",
  "isInsideOrganization": "Boolean",
  "role": "String",
  "allowedRoles": [
    "String"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarpermission"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.calendarPermission",
  "id": "2afcbc1d-bc1d-2afc-1dbc-fc2a1dbcfc2a",
  "emailAddress": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "isRemovable": "Boolean",
  "isInsideOrganization": "Boolean",
  "role": "String",
  "allowedRoles": [
    "String"
  ]
}
```

