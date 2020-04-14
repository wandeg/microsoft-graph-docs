---
title: "user: findRooms"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# findRooms

Namespace: microsoft.graph



## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions. **|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/findRooms
GET /users/{usersId}/findRooms
GET /me/managedDevices/{managedDeviceId}/users/{userId}/findRooms
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|RoomList|String||



## Response
If successful, this function returns a `200 OK` response code and a [emailAddress](../resources/emailaddress.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "user_findrooms"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='parameterValue')
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.emailaddress)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 90

{
  "value": [
    {
      "@odata.type": "microsoft.graph.emailAddress"
    }
  ]
}
```

