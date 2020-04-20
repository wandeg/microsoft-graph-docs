---
title: "Update chats"
description: "Update the properties of a chats object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update chats

Namespace: microsoft.graph

Update the properties of a chats object.

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
PATCH /me/chats
PATCH /users/{usersId}/chats
PATCH /invitations/{invitationsId}/invitedUser/chats
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [chat](../resources/chat.md) object.

The following table shows the properties that are required when you create the [chat](../resources/chat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|topic|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastUpdatedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [chat](../resources/chat.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_chats"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/chats
Content-Type: application/json
Content-length: 136

{
  "@odata.type": "#microsoft.graph.chat",
  "topic": "Topic value",
  "lastUpdatedDateTime": "2016-12-31T23:58:30.1015683+03:00"
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
  "@odata.type": "#microsoft.graph.chat",
  "id": "c30e7705-7705-c30e-0577-0ec305770ec3",
  "topic": "Topic value",
  "createdDateTime": "2016-12-31T23:57:02.5240758+03:00",
  "lastUpdatedDateTime": "2016-12-31T23:58:30.1015683+03:00"
}
```

