---
title: "Update user"
description: "Update the properties of a user object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update user

Namespace: Microsoft.AADInviteMgr

Update the properties of a [user](../resources/microsoft.aadinvitemgr-user.md) object.

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
PATCH /users/{usersId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [user](../resources/microsoft.aadinvitemgr-user.md) object.

The following table shows the properties that are required when you create the [user](../resources/microsoft.aadinvitemgr-user.md).

|Property|Type|Description|
|:---|:---|:---|



## Response
If successful, this method returns a `200 OK` response code and an updated [user](../resources/microsoft.aadinvitemgr-user.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_user"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}
Content-Type: application/json
Content-length: 53

{
  "@odata.type": "#Microsoft.AADInviteMgr.user"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#Microsoft.AADInviteMgr.user"
}
```

