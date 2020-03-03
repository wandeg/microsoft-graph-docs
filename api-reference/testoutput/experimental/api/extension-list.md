---
title: "List extensions"
description: "List properties and relationships of the extension objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List extensions

Namespace: microsoft.graph

List properties and relationships of the [extension](../resources/extension.md) objects.

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
GET /me/extensions
GET /users/{usersId}/extensions
GET /groups/{groupsId}/extensions
GET /devices/{devicesId}/extensions
GET /me/devices/{deviceId}/extensions
GET /me/messages/{messageId}/extensions
GET /me/contacts/{contactId}/extensions
GET /me/joinedGroups/{groupId}/extensions
GET /me/messages/{messageId}/event/extensions
GET /organization/{organizationId}/extensions
GET /administrativeUnits/{administrativeUnitsId}/extensions
GET /me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/extensions
GET /education/classes/{educationClassId}/members/{educationUserId}/schools/{educationSchoolId}/administrativeUnit/extensions
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [extension](../resources/extension.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_extension"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/extensions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.extension)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 141

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.extension",
      "id": "0deb773a-773a-0deb-3a77-eb0d3a77eb0d"
    }
  ]
}
```

