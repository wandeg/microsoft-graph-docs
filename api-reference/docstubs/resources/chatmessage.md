---
title: "chatMessage resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# chatMessage resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get chatMessage](../api/chatmessage-get.md)|[chatMessage](../resources/chatmessage.md)|Read the properties and relationships of a [chatMessage](../resources/chatmessage.md) object.|
|[Update chatMessage](../api/chatmessage-update.md)|[chatMessage](../resources/chatmessage.md)|Update the properties of a [chatMessage](../resources/chatmessage.md) object.|
|[delta](../api/chatmessage-delta.md)|[chatMessage](../resources/chatmessage.md) collection|**TODO: Add Description**|
|[List replies](../api/chatmessage-list-replies.md)|[chatMessage](../resources/chatmessage.md) collection|Get the chatMessages from the replies navigation property.|
|[Create replies](../api/chatmessage-post-replies.md)|[chatMessage](../resources/chatmessage.md)|Create a new replies object.|
|[Delete replies](../api/chatmessage-delete-replies.md)|None|Delete a [chatMessage](../resources/chatmessage.md) object.|
|[Update replies](../api/chatmessage-update-replies.md)|[chatMessage](../resources/chatmessage.md)|Update the properties of a replies object.|
|[Get chatMessage](../api/chatmessage-get.md)|[chatMessage](../resources/chatmessage.md)|Read the properties and relationships of a [chatMessage](../resources/chatmessage.md) object.|
|[List hostedContents](../api/chatmessage-list-hostedcontents.md)|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection|Get the chatMessageHostedContents from the hostedContents navigation property.|
|[Create hostedContents](../api/chatmessage-post-hostedcontents.md)|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)|Create a new hostedContents object.|
|[Delete hostedContents](../api/chatmessage-delete-hostedcontents.md)|None|Delete a [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.|
|[Update hostedContents](../api/chatmessage-update-hostedcontents.md)|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)|Update the properties of a hostedContents object.|
|[Get chatMessageHostedContent](../api/chatmessagehostedcontent-get.md)|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)|Read the properties and relationships of a [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attachments|[chatMessageAttachment](../resources/chatmessageattachment.md) collection|**TODO: Add Description**|
|body|[itemBody](../resources/itembody.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description**|
|etag|String|**TODO: Add Description**|
|from|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|importance|chatMessageImportance|**TODO: Add Description**. Possible values are: `normal`, `high`, `urgent`.|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|locale|String|**TODO: Add Description**|
|mentions|[chatMessageMention](../resources/chatmessagemention.md) collection|**TODO: Add Description**|
|messageType|chatMessageType|**TODO: Add Description**. Possible values are: `message`, `chatEvent`, `typing`.|
|policyViolation|[chatMessagePolicyViolation](../resources/chatmessagepolicyviolation.md)|**TODO: Add Description**|
|reactions|[chatMessageReaction](../resources/chatmessagereaction.md) collection|**TODO: Add Description**|
|replyToId|String|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|
|summary|String|**TODO: Add Description**|
|webUrl|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|hostedContents|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection|**TODO: Add Description**|
|replies|[chatMessage](../resources/chatmessage.md) collection|**TODO: Add Description**|

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

