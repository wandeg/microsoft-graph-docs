---
title: "chat resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# chat resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List chats](../api/chat-list.md)|[chat](../resources/chat.md) collection|List properties and relationships of the [chat](../resources/chat.md) objects.|
|[Get chat](../api/chat-get.md)|[chat](../resources/chat.md)|Read properties and relationships of the [chat](../resources/chat.md) object.|
|[Create chat](../api/chat-post-chats.md)|[chat](../resources/chat.md)|Create a new [chat](../resources/chat.md) object.|
|[Delete chat](../api/chat-delete.md)|None|Deletes a [chat](../resources/chat.md).|
|[Update chat](../api/chat-update.md)|[chat](../resources/chat.md)|Update the properties of a [chat](../resources/chat.md) object.|
|[allMessages](../api/chat-allmessages.md)|[chatMessage](../resources/chatmessage.md) collection||
|[List members](../api/chat-list-members.md)|[conversationMember](../resources/conversationmember.md) collection|Get the conversationMembers from the members navigation property.|
|[Add members](../api/chat-post-members.md)|[conversationMember](../resources/conversationmember.md)|Add members by posting to the members collection.|
|[List messages](../api/chat-list-messages.md)|[chatMessage](../resources/chatmessage.md) collection|Get the chatMessages from the messages navigation property.|
|[Add messages](../api/chat-post-messages.md)|[chatMessage](../resources/chatmessage.md)|Add messages by posting to the messages collection.|
|[List installedApps](../api/chat-list-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md) collection|Get the teamsAppInstallations from the installedApps navigation property.|
|[Add installedApps](../api/chat-post-installedapps.md)|[teamsAppInstallation](../resources/teamsappinstallation.md)|Add installedApps by posting to the installedApps collection.|
|[List chats](../api/user-list-chats.md)|[chat](../resources/chat.md) collection|Get the chats from the chats navigation property.|
|[Add chats](../api/user-post-chats.md)|[chat](../resources/chat.md)|Add chats by posting to the chats collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastUpdatedDateTime|DateTimeOffset||
|topic|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|installedApps|[teamsAppInstallation](../resources/teamsappinstallation.md) collection||
|members|[conversationMember](../resources/conversationmember.md) collection||
|messages|[chatMessage](../resources/chatmessage.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chat",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chat",
  "id": "String (identifier)",
  "topic": "String",
  "createdDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```

