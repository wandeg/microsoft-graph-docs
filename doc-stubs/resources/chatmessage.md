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


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List messages](../api/channel-list-messages.md)|[chatMessage](../resources/chatmessage.md) collection|Get the chatMessages from the messages navigation property.|
|[Create messages](../api/channel-post-messages.md)|[chatMessage](../resources/chatmessage.md)|Create a new messages object.|
|[Delete messages](../api/channel-delete-messages.md)|None|Delete a [chatMessage](../resources/chatmessage.md) object.|
|[Update messages](../api/channel-update-messages.md)|[chatMessage](../resources/chatmessage.md)|Update the properties of a messages object.|
|[Get messages](../api/channel-get-chatmessage.md)|[chatMessage](../resources/chatmessage.md)|Read the properties and relationships of a [chatMessage](../resources/chatmessage.md) object.|
|[List replies](../api/chatmessage-list-replies.md)|[chatMessage](../resources/chatmessage.md) collection|Get the chatMessages from the replies navigation property.|
|[Create replies](../api/chatmessage-post-replies.md)|[chatMessage](../resources/chatmessage.md)|Create a new replies object.|
|[Delete replies](../api/chatmessage-delete-replies.md)|None|Delete a [chatMessage](../resources/chatmessage.md) object.|
|[Update replies](../api/chatmessage-update-replies.md)|[chatMessage](../resources/chatmessage.md)|Update the properties of a replies object.|
|[Get replies](../api/chatmessage-get-chatmessage.md)|[chatMessage](../resources/chatmessage.md)|Read the properties and relationships of a [chatMessage](../resources/chatmessage.md) object.|
|[List hostedContents](../api/chatmessage-list-hostedcontents.md)|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md) collection|Get the chatMessageHostedContents from the hostedContents navigation property.|
|[Create hostedContents](../api/chatmessage-post-hostedcontents.md)|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)|Create a new hostedContents object.|
|[Delete hostedContents](../api/chatmessage-delete-hostedcontents.md)|None|Delete a [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.|
|[Update hostedContents](../api/chatmessage-update-hostedcontents.md)|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)|Update the properties of a hostedContents object.|
|[Get hostedContents](../api/chatmessage-get-chatmessagehostedcontent.md)|[chatMessageHostedContent](../resources/chatmessagehostedcontent.md)|Read the properties and relationships of a [chatMessageHostedContent](../resources/chatmessagehostedcontent.md) object.|

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
|importance|chatMessageImportance|**TODO: Add Description**. Possible values are: `normal`, `high`, `urgent`, `unknownFutureValue`.|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|locale|String|**TODO: Add Description**|
|mentions|[chatMessageMention](../resources/chatmessagemention.md) collection|**TODO: Add Description**|
|messageType|chatMessageType|**TODO: Add Description**. Possible values are: `message`, `chatEvent`, `typing`, `unknownFutureValue`.|
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
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.identitySet"
  },
  "etag": "String",
  "messageType": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "subject": "String",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "summary": "String",
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
  "locale": "String",
  "webUrl": "String"
}
```

