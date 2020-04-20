---
title: "Delete mobileAppTroubleshootingEvents"
description: "Delete a mobileAppTroubleshootingEvents object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Delete mobileAppTroubleshootingEvents

Namespace: microsoft.graph

Delete a mobileAppTroubleshootingEvents object.

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
DELETE /me/mobileAppTroubleshootingEvents
DELETE /users/{usersId}/mobileAppTroubleshootingEvents
DELETE /invitations/{invitationsId}/invitedUser/mobileAppTroubleshootingEvents
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `204 No Content` response code.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "delete_mobileapptroubleshootingevents_from_user"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/mobileAppTroubleshootingEvents
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

