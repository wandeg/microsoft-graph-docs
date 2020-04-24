---
title: "List messages"
description: "Get the chatMessages from the messages navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List messages

Namespace: microsoft.graph

Get the chatMessages from the messages navigation property.

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
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/channels/{channelId}/messages
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [chatMessage](../resources/chatmessage.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_chatmessage"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/channels/{channelId}/messages
```

### Response
**Note:** The response object shown here might be shortened for readability.
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
  ]
}
```

