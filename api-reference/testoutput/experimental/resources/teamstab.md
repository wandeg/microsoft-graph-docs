---
title: "teamsTab resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# teamsTab resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get teamsTab](../api/teamstab-get.md)|[teamsTab](../resources/teamsTab.md)|Read properties and relationships of the [teamsTab](../resources/teamstab.md) object.|
|[Delete teamsTab](../api/teamstab-delete.md)|None|Deletes a [teamsTab](../resources/teamstab.md).|
|[Update teamsTab](../api/teamstab-update.md)|[teamsTab](../resources/teamsTab.md)|Update the properties of a [teamsTab](../resources/teamstab.md) object.|
|[Get teamsApp](../api/teamsapp-get.md)|[teamsApp](../resources/teamsApp.md)|Read properties and relationships of the [teamsApp](../resources/teamsapp.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|configuration|[teamsTabConfiguration](../resources/teamsTabConfiguration.md)||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|messageId|String||
|name|String||
|sortOrderIndex|String||
|teamsAppId|String||
|webUrl|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|teamsApp|[teamsApp](../resources/teamsApp.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsTab",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsTab",
  "id": "String (identifier)",
  "name": "String",
  "displayName": "String",
  "teamsAppId": "String",
  "sortOrderIndex": "String",
  "messageId": "String",
  "webUrl": "String",
  "configuration": {
    "@odata.type": "microsoft.graph.teamsTabConfiguration",
    "entityId": "String",
    "contentUrl": "String",
    "removeUrl": "String",
    "websiteUrl": "String"
  }
}
```

