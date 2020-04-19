---
title: "team: allMessages"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# allMessages

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /teams/allMessages
GET /users/{usersId}/joinedTeams/allMessages
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [chatMessage](../resources/chatmessage.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "team_allmessages"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/allMessages
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.chatmessage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.chatMessage",
      "id": "2e2a23df-23df-2e2a-df23-2a2edf232a2e",
      "replyToId": "Reply To Id value",
      "from": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "etag": "Etag value",
      "messageType": "String",
      "createdDateTime": "2017-01-01T00:00:27.9270493+03:00",
      "lastModifiedDateTime": "2017-01-01T00:00:12.2512781+03:00",
      "deletedDateTime": "2017-01-01T00:03:11.3808645+03:00",
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

