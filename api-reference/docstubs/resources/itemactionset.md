---
title: "itemActionSet resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# itemActionSet resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|comment|[commentAction](../resources/commentaction.md)|**TODO: Add Description**|
|create|[createAction](../resources/createaction.md)|**TODO: Add Description**|
|delete|[deleteAction](../resources/deleteaction.md)|**TODO: Add Description**|
|edit|[editAction](../resources/editaction.md)|**TODO: Add Description**|
|mention|[mentionAction](../resources/mentionaction.md)|**TODO: Add Description**|
|move|[moveAction](../resources/moveaction.md)|**TODO: Add Description**|
|rename|[renameAction](../resources/renameaction.md)|**TODO: Add Description**|
|restore|[restoreAction](../resources/restoreaction.md)|**TODO: Add Description**|
|share|[shareAction](../resources/shareaction.md)|**TODO: Add Description**|
|version|[versionAction](../resources/versionaction.md)|**TODO: Add Description**|

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

