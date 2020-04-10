---
title: "itemActivityOLD resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# itemActivityOLD resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get itemActivityOLD](../api/itemactivityold-get.md)|[itemActivityOLD](../resources/itemactivityold.md)|Read properties and relationships of the [itemActivityOLD](../resources/itemactivityold.md) object.|
|[Update itemActivityOLD](../api/itemactivityold-update.md)|[itemActivityOLD](../resources/itemactivityold.md)|Update the properties of a [itemActivityOLD](../resources/itemactivityold.md) object.|
|[Get driveItem](../api/driveitem-get.md)|[driveItem](../resources/driveitem.md)|Read properties and relationships of the [driveItem](../resources/driveitem.md) object.|
|[Get listItem](../api/listitem-get.md)|[listItem](../resources/listitem.md)|Read properties and relationships of the [listItem](../resources/listitem.md) object.|
|[List activities](../api/drive-list-activities.md)|[itemActivityOLD](../resources/itemactivityold.md) collection|Get the itemActivityOLDs from the activities navigation property.|
|[Add activities](../api/drive-post-activities.md)|[itemActivityOLD](../resources/itemactivityold.md)|Add activities by posting to the activities collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|action|[itemActionSet](../resources/itemactionset.md)||
|actor|[identitySet](../resources/identityset.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|times|[itemActivityTimeSet](../resources/itemactivitytimeset.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|driveItem|[driveItem](../resources/driveitem.md)||
|listItem|[listItem](../resources/listitem.md)||

## JSON representation
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

