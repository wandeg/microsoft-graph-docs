---
title: "Add messages"
description: "Add messages by posting to the messages collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add messages

Namespace: microsoft.graph

Add messages by posting to the messages collection.

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
POST /chats/{chatsId}/messages/$ref
POST /me/chats/{chatId}/messages/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [chatMessage](../resources/chatmessage.md) object.

The following table shows the properties that are required when you create the [chatMessage](../resources/chatmessage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|replyToId|String||
|from|[identitySet](../resources/identityset.md)||
|etag|String||
|messageType|Enumeration| Possible values are: `message`, `chatEvent`, `typing`.|
|createdDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||
|deletedDateTime|DateTimeOffset||
|subject|String||
|body|[itemBody](../resources/itembody.md)||
|summary|String||
|attachments|[chatMessageAttachment](../resources/chatmessageattachment.md) collection||
|mentions|[chatMessageMention](../resources/chatmessagemention.md) collection||
|importance|Enumeration| Possible values are: `normal`, `high`, `urgent`.|
|policyViolation|[chatMessagePolicyViolation](../resources/chatmessagepolicyviolation.md)||
|reactions|[chatMessageReaction](../resources/chatmessagereaction.md) collection||
|locale|String||
|webUrl|String||



## Response
If successful, this method returns a `201 Created` response code and a [chatMessage](../resources/chatmessage.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/chats/{chatsId}/messages
Content-type: application/json
Content-length: 2162

{
  "@odata.type": "#microsoft.graph.chatMessage",
  "replyToId": "Reply To Id value",
  "from": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "etag": "Etag value",
  "messageType": "String",
  "deletedDateTime": "2017-01-01T00:02:56.4302403+03:00",
  "subject": "Subject value",
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "Content value"
  },
  "summary": "Summary value",
  "attachments": [
    {
      "@odata.type": "microsoft.graph.chatMessageAttachment",
      "contentType": "Content Type value",
      "contentUrl": "https://example.com/contentUrl/",
      "name": "Name value",
      "thumbnailUrl": "https://example.com/thumbnailUrl/"
    }
  ],
  "mentions": [
    {
      "@odata.type": "microsoft.graph.chatMessageMention",
      "id": 2,
      "mentionText": "Mention Text value",
      "mentioned": {
        "@odata.type": "microsoft.graph.identitySet"
      }
    }
  ],
  "importance": "String",
  "policyViolation": {
    "@odata.type": "microsoft.graph.chatMessagePolicyViolation",
    "dlpAction": "String",
    "justificationText": "Justification Text value",
    "policyTip": {
      "@odata.type": "microsoft.graph.chatMessagePolicyViolationPolicyTip",
      "generalText": "General Text value",
      "complianceUrl": "https://example.com/complianceUrl/",
      "matchedConditionDescriptions": [
        "Matched Condition Descriptions value"
      ]
    },
    "userAction": "String",
    "verdictDetails": "String"
  },
  "reactions": [
    {
      "@odata.type": "microsoft.graph.chatMessageReaction",
      "reactionType": "Reaction Type value",
      "user": {
        "@odata.type": "microsoft.graph.identitySet"
      }
    }
  ],
  "locale": "Locale value",
  "webUrl": "https://example.com/webUrl/"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatmessage"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2333

{
  "@odata.type": "#microsoft.graph.chatMessage",
  "id": "bc32114e-114e-bc32-4e11-32bc4e1132bc",
  "replyToId": "Reply To Id value",
  "from": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "etag": "Etag value",
  "messageType": "String",
  "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
  "deletedDateTime": "2017-01-01T00:02:56.4302403+03:00",
  "subject": "Subject value",
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "Content value"
  },
  "summary": "Summary value",
  "attachments": [
    {
      "@odata.type": "microsoft.graph.chatMessageAttachment",
      "contentType": "Content Type value",
      "contentUrl": "https://example.com/contentUrl/",
      "name": "Name value",
      "thumbnailUrl": "https://example.com/thumbnailUrl/"
    }
  ],
  "mentions": [
    {
      "@odata.type": "microsoft.graph.chatMessageMention",
      "id": 2,
      "mentionText": "Mention Text value",
      "mentioned": {
        "@odata.type": "microsoft.graph.identitySet"
      }
    }
  ],
  "importance": "String",
  "policyViolation": {
    "@odata.type": "microsoft.graph.chatMessagePolicyViolation",
    "dlpAction": "String",
    "justificationText": "Justification Text value",
    "policyTip": {
      "@odata.type": "microsoft.graph.chatMessagePolicyViolationPolicyTip",
      "generalText": "General Text value",
      "complianceUrl": "https://example.com/complianceUrl/",
      "matchedConditionDescriptions": [
        "Matched Condition Descriptions value"
      ]
    },
    "userAction": "String",
    "verdictDetails": "String"
  },
  "reactions": [
    {
      "@odata.type": "microsoft.graph.chatMessageReaction",
      "reactionType": "Reaction Type value",
      "user": {
        "@odata.type": "microsoft.graph.identitySet"
      }
    }
  ],
  "locale": "Locale value",
  "webUrl": "https://example.com/webUrl/"
}
```

