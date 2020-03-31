---
title: "delta"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# delta

Namespace: microsoft.graph



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
GET /chats/{chatsId}/messages/delta
GET /me/chats/{chatId}/messages/delta
GET /me/joinedGroups/{groupId}/team/channels/{channelId}/messages/delta
GET /me/joinedGroups/{groupId}/team/channels/{channelId}/messages/{chatMessageId}/replies/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [chatMessage](../resources/chatmessage.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "chatmessage_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/chats/{chatsId}/messages/delta
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.chatmessage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1242

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.chatMessage",
      "id": "bc32114e-114e-bc32-4e11-32bc4e1132bc",
      "replyToId": "Reply To Id value",
      "from": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "etag": "Etag value",
      "messageType": "String",
      "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
      "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
      "deletedDateTime": "2017-01-01T00:02:56.4302403+03:00",
      "subject": "Subject value",
      "body": {
        "@odata.type": "microsoft.graph.itemBody"
      },
      "summary": "Summary value",
      "attachments": [
        {
          "@odata.type": "microsoft.graph.chatMessageAttachment"
        }
      ],
      "mentions": [
        {
          "@odata.type": "microsoft.graph.chatMessageMention"
        }
      ],
      "importance": "String",
      "policyViolation": {
        "@odata.type": "microsoft.graph.chatMessagePolicyViolation"
      },
      "reactions": [
        {
          "@odata.type": "microsoft.graph.chatMessageReaction"
        }
      ],
      "locale": "Locale value",
      "webUrl": "https://example.com/webUrl/"
    }
  ]
}
```

