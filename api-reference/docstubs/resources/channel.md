---
title: "channel resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# channel resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get channel](../api/channel-get.md)|[channel](../resources/channel.md)|Read the properties and relationships of a [channel](../resources/channel.md) object.|
|[Update channel](../api/channel-update.md)|[channel](../resources/channel.md)|Update the properties of a [channel](../resources/channel.md) object.|
|[List messages](../api/channel-list-messages.md)|[chatMessage](../resources/chatmessage.md) collection|Get the chatMessages from the messages navigation property.|
|[Create messages](../api/channel-post-messages.md)|[chatMessage](../resources/chatmessage.md)|Create a new messages object.|
|[Delete messages](../api/channel-delete-messages.md)|None|Delete a [chatMessage](../resources/chatmessage.md) object.|
|[Update messages](../api/channel-update-messages.md)|[chatMessage](../resources/chatmessage.md)|Update the properties of a messages object.|
|[Get chatMessage](../api/chatmessage-get.md)|[chatMessage](../resources/chatmessage.md)|Read the properties and relationships of a [chatMessage](../resources/chatmessage.md) object.|
|[List tabs](../api/channel-list-tabs.md)|[teamsTab](../resources/teamstab.md) collection|Get the teamsTabs from the tabs navigation property.|
|[Create tabs](../api/channel-post-tabs.md)|[teamsTab](../resources/teamstab.md)|Create a new tabs object.|
|[Delete tabs](../api/channel-delete-tabs.md)|None|Delete a [teamsTab](../resources/teamstab.md) object.|
|[Update tabs](../api/channel-update-tabs.md)|[teamsTab](../resources/teamstab.md)|Update the properties of a tabs object.|
|[Get teamsTab](../api/teamstab-get.md)|[teamsTab](../resources/teamstab.md)|Read the properties and relationships of a [teamsTab](../resources/teamstab.md) object.|
|[List members](../api/channel-list-members.md)|[conversationMember](../resources/conversationmember.md) collection|Get the conversationMembers from the members navigation property.|
|[Create members](../api/channel-post-members.md)|[conversationMember](../resources/conversationmember.md)|Create a new members object.|
|[Delete members](../api/channel-delete-members.md)|None|Delete a [conversationMember](../resources/conversationmember.md) object.|
|[Update members](../api/channel-update-members.md)|[conversationMember](../resources/conversationmember.md)|Update the properties of a members object.|
|[Get conversationMember](../api/conversationmember-get.md)|[conversationMember](../resources/conversationmember.md)|Read the properties and relationships of a [conversationMember](../resources/conversationmember.md) object.|
|[List filesFolder](../api/channel-list-filesfolder.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItems from the filesFolder navigation property.|
|[Create filesFolder](../api/channel-post-filesfolder.md)|[driveItem](../resources/driveitem.md)|Create a new filesFolder object.|
|[Delete filesFolder](../api/channel-delete-filesfolder.md)|None|Delete a [driveItem](../resources/driveitem.md) object.|
|[Update filesFolder](../api/channel-update-filesfolder.md)|[driveItem](../resources/driveitem.md)|Update the properties of a filesFolder object.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveitem.md)|Read the properties and relationships of a [driveItem](../resources/driveitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isFavoriteByDefault|Boolean|**TODO: Add Description**|
|membershipType|channelMembershipType|**TODO: Add Description**. Possible values are: `standard`, `private`, `unknownFutureValue`.|
|webUrl|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|filesFolder|[driveItem](../resources/driveitem.md)|**TODO: Add Description**|
|members|[conversationMember](../resources/conversationmember.md) collection|**TODO: Add Description**|
|messages|[chatMessage](../resources/chatmessage.md) collection|**TODO: Add Description**|
|tabs|[teamsTab](../resources/teamstab.md) collection|**TODO: Add Description**|

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

