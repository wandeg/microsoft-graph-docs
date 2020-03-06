---
title: "chatMessage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# chatMessage resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get chatMessage](../api/chatmessage-get.md)|[chatMessage](../resources/chatmessage.md)|Read properties and relationships of the [chatMessage](../resources/chatmessage.md) object.|
|[Update chatMessage](../api/chatmessage-update.md)|[chatMessage](../resources/chatmessage.md)|Update the properties of a [chatMessage](../resources/chatmessage.md) object.|
|[delta](../api/chatmessage-delta.md)|[chatMessage](../resources/chatmessage.md) collection||
|[List replies](../api/chatmessage-list-replies.md)|[chatMessage](../resources/chatmessage.md) collection|Get the chatMessages from the replies navigation property.|
|[Add replies](../api/chatmessage-post-replies.md)|[chatMessage](../resources/chatmessage.md)|Add replies by posting to the replies collection.|
|[List hostedContents](../api/chatmessage-list-hostedcontents.md)|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection|Get the chatMessageHostedContents from the hostedContents navigation property.|
|[Add hostedContents](../api/chatmessage-post-hostedcontents.md)|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)|Add hostedContents by posting to the hostedContents collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attachments|[chatMessageAttachment](../resources/chatmessageattachment.md) collection||
|body|[itemBody](../resources/itembody.md)||
|createdDateTime|DateTimeOffset||
|deletedDateTime|DateTimeOffset||
|etag|String||
|from|[identitySet](../resources/identityset.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|importance|Enumeration|. Possible values are: `normal`, `high`, `urgent`.|
|lastModifiedDateTime|DateTimeOffset||
|locale|String||
|mentions|[chatMessageMention](../resources/chatmessagemention.md) collection||
|messageType|Enumeration|. Possible values are: `message`, `chatEvent`, `typing`.|
|policyViolation|[chatMessagePolicyViolation](../resources/chatmessagepolicyviolation.md)||
|reactions|[chatMessageReaction](../resources/chatmessagereaction.md) collection||
|replyToId|String||
|subject|String||
|summary|String||
|webUrl|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|hostedContents|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection||
|replies|[chatMessage](../resources/chatmessage.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessage",
  "id": "String (identifier)",
  "replyToId": "String",
  "from": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "etag": "String",
  "messageType": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "subject": "String",
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "String"
  },
  "summary": "String",
  "attachments": [
    {
      "@odata.type": "microsoft.graph.chatMessageAttachment",
      "contentType": "String",
      "contentUrl": "String",
      "name": "String",
      "thumbnailUrl": "String"
    }
  ],
  "mentions": [
    {
      "@odata.type": "microsoft.graph.chatMessageMention",
      "id": 1024,
      "mentionText": "String",
      "mentioned": {
        "@odata.type": "microsoft.graph.identitySet"
      }
    }
  ],
  "importance": "String",
  "policyViolation": {
    "@odata.type": "microsoft.graph.chatMessagePolicyViolation",
    "dlpAction": "String",
    "justificationText": "String",
    "policyTip": {
      "@odata.type": "microsoft.graph.chatMessagePolicyViolationPolicyTip",
      "generalText": "String",
      "complianceUrl": "String",
      "matchedConditionDescriptions": [
        "String"
      ]
    },
    "userAction": "String",
    "verdictDetails": "String"
  },
  "reactions": [
    {
      "@odata.type": "microsoft.graph.chatMessageReaction",
      "reactionType": "String",
      "user": {
        "@odata.type": "microsoft.graph.identitySet"
      }
    }
  ],
  "locale": "String",
  "webUrl": "String"
}
```

