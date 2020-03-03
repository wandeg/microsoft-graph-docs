---
title: "itemActionSet resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# itemActionSet resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|comment|[commentAction](../resources/commentAction.md)||
|create|[createAction](../resources/createAction.md)||
|delete|[deleteAction](../resources/deleteAction.md)||
|edit|[editAction](../resources/editAction.md)||
|mention|[mentionAction](../resources/mentionAction.md)||
|move|[moveAction](../resources/moveAction.md)||
|rename|[renameAction](../resources/renameAction.md)||
|restore|[restoreAction](../resources/restoreAction.md)||
|share|[shareAction](../resources/shareAction.md)||
|version|[versionAction](../resources/versionAction.md)||

## Relationships
None

## JSON Representation
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

