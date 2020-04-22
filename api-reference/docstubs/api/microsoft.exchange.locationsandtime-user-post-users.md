---
title: "Create user"
description: "Create a new user object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create user

Namespace: microsoft.exchange.locationsAndTime

Create a new [user](../resources/microsoft.exchange.locationsandtime-user.md) object.

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
POST /users
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [user](../resources/microsoft.exchange.locationsandtime-user.md) object.

The following table shows the properties that are required when you create the [user](../resources/microsoft.exchange.locationsandtime-user.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [user](../resources/microsoft.exchange.locationsandtime-user.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}
-->
``` http
POST https://graph.microsoft.com/beta/users
Content-Type: application/json
Content-length: 66

{
  "@odata.type": "#microsoft.exchange.locationsAndTime.user"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.exchange.locationsandtime.user"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.exchange.locationsAndTime.user",
  "id": "1f2c8108-8108-1f2c-0881-2c1f08812c1f"
}
```

