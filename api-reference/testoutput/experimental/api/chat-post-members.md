---
title: "Add members"
description: "Add members by posting to the members collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add members

Add members by posting to the members collection.

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
POST /chats/{chatsId}/members/$ref
POST /me/chats/{chatId}/members/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the conversationMember object.

The following table shows the properties that are required when you create the conversationMember.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|roles|String collection||
|displayName|String||



## Response
If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_conversationmember_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/chats/{chatsId}/members
Content-type: application/json
Content-length: 139

{
  "@odata.type": "#microsoft.graph.conversationMember",
  "roles": [
    "Roles value"
  ],
  "displayName": "Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationmember"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 188

{
  "@odata.type": "#microsoft.graph.conversationMember",
  "id": "15f74870-4870-15f7-7048-f7157048f715",
  "roles": [
    "Roles value"
  ],
  "displayName": "Display Name value"
}
```

