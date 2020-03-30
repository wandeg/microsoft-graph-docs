---
title: "channel resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# channel resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get channel](../api/channel-get.md)|[channel](../resources/channel.md)|Read properties and relationships of the [channel](../resources/channel.md) object.|
|[Update channel](../api/channel-update.md)|[channel](../resources/channel.md)|Update the properties of a [channel](../resources/channel.md) object.|
|[List messages](../api/channel-list-messages.md)|[chatMessage](../resources/chatmessage.md) collection|Get the chatMessages from the messages navigation property.|
|[Add messages](../api/channel-post-messages.md)|[chatMessage](../resources/chatmessage.md)|Add messages by posting to the messages collection.|
|[List tabs](../api/channel-list-tabs.md)|[teamsTab](../resources/teamstab.md) collection|Get the teamsTabs from the tabs navigation property.|
|[Add tabs](../api/channel-post-tabs.md)|[teamsTab](../resources/teamstab.md)|Add tabs by posting to the tabs collection.|
|[List members](../api/channel-list-members.md)|[conversationMember](../resources/conversationmember.md) collection|Get the conversationMembers from the members navigation property.|
|[Add members](../api/channel-post-members.md)|[conversationMember](../resources/conversationmember.md)|Add members by posting to the members collection.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveitem.md)|Read properties and relationships of the [driveItem](../resources/driveitem.md) object.|
|[List channels](../api/team-list-channels.md)|[channel](../resources/channel.md) collection|Get the channels from the channels navigation property.|
|[Add channels](../api/team-post-channels.md)|[channel](../resources/channel.md)|Add channels by posting to the channels collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|displayName|String||
|email|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isFavoriteByDefault|Boolean||
|membershipType|Enumeration| Possible values are: `standard`, `private`, `unknownFutureValue`.|
|webUrl|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|filesFolder|[driveItem](../resources/driveitem.md)||
|members|[conversationMember](../resources/conversationmember.md) collection||
|messages|[chatMessage](../resources/chatmessage.md) collection||
|tabs|[teamsTab](../resources/teamstab.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.channel",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channel",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isFavoriteByDefault": true,
  "email": "String",
  "webUrl": "String",
  "membershipType": "String"
}
```

