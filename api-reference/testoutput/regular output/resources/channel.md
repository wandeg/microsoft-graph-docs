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
|[List channels](../api/channel-list.md)|[channel](../resources/channel.md) collection|List properties and relationships of the [channel](../resources/channel.md) objects.|
|[Get channel](../api/channel-get.md)|[channel](../resources/channel.md)|Read properties and relationships of the [channel](../resources/channel.md) object.|
|[Create channel](../api/channel-create.md)|[channel](../resources/channel.md)|Create a new [channel](../resources/channel.md) object.|
|[Delete channel](../api/channel-delete.md)|None|Deletes a [channel](../resources/channel.md).|
|[Update channel](../api/channel-update.md)|[channel](../resources/channel.md)|Update the properties of a [channel](../resources/channel.md) object.|
|[List tabs](../api/channel-list-tabs.md)|[teamsTab](../resources/teamstab.md) collection|Get the teamsTabs from the tabs navigation property.|
|[Add tabs](../api/channel-post-tabs.md)|[teamsTab](../resources/teamstab.md)|Add tabs by posting to the tabs collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|displayName|String||
|email|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|webUrl|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|tabs|[teamsTab](../resources/teamstab.md) collection||

## JSON Representation
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
  "email": "String",
  "webUrl": "String"
}
```

