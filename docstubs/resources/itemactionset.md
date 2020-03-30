---
title: "itemActionSet resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# itemActionSet resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|comment|[commentAction](../resources/commentaction.md)||
|create|[createAction](../resources/createaction.md)||
|delete|[deleteAction](../resources/deleteaction.md)||
|edit|[editAction](../resources/editaction.md)||
|mention|[mentionAction](../resources/mentionaction.md)||
|move|[moveAction](../resources/moveaction.md)||
|rename|[renameAction](../resources/renameaction.md)||
|restore|[restoreAction](../resources/restoreaction.md)||
|share|[shareAction](../resources/shareaction.md)||
|version|[versionAction](../resources/versionaction.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.itemActionSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemActionSet",
  "comment": {
    "@odata.type": "microsoft.graph.commentAction",
    "isReply": true,
    "parentAuthor": {
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
    "name": "String",
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
}
```

