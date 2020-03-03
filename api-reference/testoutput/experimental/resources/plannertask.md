---
title: "plannerTask resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# plannerTask resource type




Inherits from [plannerDelta](../resources/plannerDelta.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get plannerTask](../api/plannertask-get.md)|[plannerTask](../resources/plannerTask.md)|Read properties and relationships of the [plannerTask](../resources/plannertask.md) object.|
|[Delete plannerTask](../api/plannertask-delete.md)|None|Deletes a [plannerTask](../resources/plannertask.md).|
|[Update plannerTask](../api/plannertask-update.md)|[plannerTask](../resources/plannerTask.md)|Update the properties of a [plannerTask](../resources/plannertask.md) object.|
|[Get plannerTaskDetails](../api/plannertaskdetails-get.md)|[plannerTaskDetails](../resources/plannerTaskDetails.md)|Read properties and relationships of the [plannerTaskDetails](../resources/plannertaskdetails.md) object.|
|[Get plannerAssignedToTaskBoardTaskFormat](../api/plannerassignedtotaskboardtaskformat-get.md)|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerAssignedToTaskBoardTaskFormat.md)|Read properties and relationships of the [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object.|
|[Get plannerProgressTaskBoardTaskFormat](../api/plannerprogresstaskboardtaskformat-get.md)|[plannerProgressTaskBoardTaskFormat](../resources/plannerProgressTaskBoardTaskFormat.md)|Read properties and relationships of the [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object.|
|[Get plannerBucketTaskBoardTaskFormat](../api/plannerbuckettaskboardtaskformat-get.md)|[plannerBucketTaskBoardTaskFormat](../resources/plannerBucketTaskBoardTaskFormat.md)|Read properties and relationships of the [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeChecklistItemCount|Int32||
|appliedCategories|[plannerAppliedCategories](../resources/plannerAppliedCategories.md)||
|assigneePriority|String||
|assignments|[plannerAssignments](../resources/plannerAssignments.md)||
|bucketId|String||
|checklistItemCount|Int32||
|completedBy|[identitySet](../resources/identitySet.md)||
|completedDateTime|DateTimeOffset||
|conversationThreadId|String||
|createdBy|[identitySet](../resources/identitySet.md)||
|createdDateTime|DateTimeOffset||
|dueDateTime|DateTimeOffset||
|hasDescription|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|orderHint|String||
|percentComplete|Int32||
|planId|String||
|previewType|Enumeration|. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.|
|priority|Int32||
|referenceCount|Int32||
|startDateTime|DateTimeOffset||
|title|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignedToTaskBoardFormat|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerAssignedToTaskBoardTaskFormat.md)||
|bucketTaskBoardFormat|[plannerBucketTaskBoardTaskFormat](../resources/plannerBucketTaskBoardTaskFormat.md)||
|details|[plannerTaskDetails](../resources/plannerTaskDetails.md)||
|progressTaskBoardFormat|[plannerProgressTaskBoardTaskFormat](../resources/plannerProgressTaskBoardTaskFormat.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerTask",
  "baseType": "microsoft.graph.plannerDelta",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerTask",
  "id": "String (identifier)",
  "createdBy": {
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
  "planId": "String",
  "bucketId": "String",
  "title": "String",
  "orderHint": "String",
  "assigneePriority": "String",
  "percentComplete": 1024,
  "priority": 1024,
  "startDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "hasDescription": true,
  "previewType": "String",
  "completedDateTime": "String (timestamp)",
  "completedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "referenceCount": 1024,
  "checklistItemCount": 1024,
  "activeChecklistItemCount": 1024,
  "appliedCategories": {
    "@odata.type": "microsoft.graph.plannerAppliedCategories"
  },
  "assignments": {
    "@odata.type": "microsoft.graph.plannerAssignments"
  },
  "conversationThreadId": "String"
}
```

