---
title: "itemActivityOLD resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# itemActivityOLD resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get itemActivityOLD](../api/itemactivityold-get.md)|[itemActivityOLD](../resources/itemActivityOLD.md)|Read properties and relationships of the [itemActivityOLD](../resources/itemactivityold.md) object.|
|[Delete itemActivityOLD](../api/itemactivityold-delete.md)|None|Deletes a [itemActivityOLD](../resources/itemactivityold.md).|
|[Update itemActivityOLD](../api/itemactivityold-update.md)|[itemActivityOLD](../resources/itemActivityOLD.md)|Update the properties of a [itemActivityOLD](../resources/itemactivityold.md) object.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveItem.md)|Read properties and relationships of the [driveItem](../resources/driveitem.md) object.|
|[Get listItem](../api/listitem-get.md)|[listItem](../resources/listItem.md)|Read properties and relationships of the [listItem](../resources/listitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|[itemActionSet](../resources/itemActionSet.md)||
|actor|[identitySet](../resources/identitySet.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|times|[itemActivityTimeSet](../resources/itemActivityTimeSet.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|driveItem|[driveItem](../resources/driveItem.md)||
|listItem|[listItem](../resources/listItem.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemActivityOLD",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemActivityOLD",
  "id": "String (identifier)",
  "action": {
    "@odata.type": "microsoft.graph.itemActionSet",
    "comment": {
      "@odata.type": "microsoft.graph.commentAction",
      "isReply": true,
      "parentAuthor": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "participants": [
        {
          "@odata.type": "microsoft.graph.identitySet"
        }
      ]
    },
    "create": {
      "@odata.type": "microsoft.graph.createAction"
    },
    "delete": {
      "@odata.type": "microsoft.graph.deleteAction",
      "objectType": "String"
    },
    "edit": {
      "@odata.type": "microsoft.graph.editAction"
    },
    "mention": {
      "@odata.type": "microsoft.graph.mentionAction",
      "mentionees": [
        {
          "@odata.type": "microsoft.graph.identitySet"
        }
      ]
    },
    "move": {
      "@odata.type": "microsoft.graph.moveAction",
      "from": "String",
      "to": "String"
    },
    "rename": {
      "@odata.type": "microsoft.graph.renameAction",
      "newName": "String",
      "oldName": "String"
    },
    "restore": {
      "@odata.type": "microsoft.graph.restoreAction"
    },
    "share": {
      "@odata.type": "microsoft.graph.shareAction",
      "recipients": [
        {
          "@odata.type": "microsoft.graph.identitySet"
        }
      ]
    },
    "version": {
      "@odata.type": "microsoft.graph.versionAction",
      "newVersion": "String"
    }
  },
  "actor": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "times": {
    "@odata.type": "microsoft.graph.itemActivityTimeSet",
    "lastRecordedDateTime": "String (timestamp)",
    "observedDateTime": "String (timestamp)",
    "recordedDateTime": "String (timestamp)"
  }
}
```

