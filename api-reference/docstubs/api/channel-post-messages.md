---
title: "Create messages"
description: "Create a new messages object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create messages

Namespace: microsoft.graph

Create a new messages object.

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
POST /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/channels/{channelId}/messages
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [chatMessage](../resources/chatmessage.md) object.

The following table shows the properties that are required when you create the [chatMessage](../resources/chatmessage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|replyToId|String|**TODO: Add Description**|
|from|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|etag|String|**TODO: Add Description**|
|messageType|chatMessageType|**TODO: Add Description**. Possible values are: `message`, `chatEvent`, `typing`.|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|
|body|[itemBody](../resources/itembody.md)|**TODO: Add Description**|
|summary|String|**TODO: Add Description**|
|attachments|[chatMessageAttachment](../resources/chatmessageattachment.md) collection|**TODO: Add Description**|
|mentions|[chatMessageMention](../resources/chatmessagemention.md) collection|**TODO: Add Description**|
|importance|chatMessageImportance|**TODO: Add Description**. Possible values are: `normal`, `high`, `urgent`.|
|policyViolation|[chatMessagePolicyViolation](../resources/chatmessagepolicyviolation.md)|**TODO: Add Description**|
|reactions|[chatMessageReaction](../resources/chatmessagereaction.md) collection|**TODO: Add Description**|
|locale|String|**TODO: Add Description**|
|webUrl|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [chatMessage](../resources/chatmessage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/channels/{channelId}/messages
Content-Type: application/json
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
  "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00",
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatmessage"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.chatMessage",
  "id": "8d46bb0d-bb0d-8d46-0dbb-468d0dbb468d",
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
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00",
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

