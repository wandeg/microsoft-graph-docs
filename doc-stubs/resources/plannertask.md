---
title: "plannerTask resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# plannerTask resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List tasks](../api/planneruser-list-tasks.md)|[plannerTask](../resources/plannertask.md) collection|Get the plannerTasks from the tasks navigation property.|
|[Add tasks](../api/planneruser-post-tasks.md)|[plannerTask](../resources/plannertask.md)|Add tasks by posting to the tasks collection.|
|[Remove tasks](../api/planneruser-delete-tasks.md)|None|Remove a [plannerTask](../resources/plannertask.md) object.|
|[List details](../api/plannertask-list-details.md)|[plannerTaskDetails](../resources/plannertaskdetails.md) collection|Get the plannerTaskDetails from the details navigation property.|
|[Create details](../api/plannertask-post-details.md)|[plannerTaskDetails](../resources/plannertaskdetails.md)|Create a new details object.|
|[Delete details](../api/plannertask-delete-details.md)|None|Delete a [plannerTaskDetails](../resources/plannertaskdetails.md) object.|
|[Update details](../api/plannertask-update-details.md)|[plannerTaskDetails](../resources/plannertaskdetails.md)|Update the properties of a details object.|
|[Get details](../api/plannertask-get-plannertaskdetails.md)|[plannerTaskDetails](../resources/plannertaskdetails.md)|Read the properties and relationships of a [plannerTaskDetails](../resources/plannertaskdetails.md) object.|
|[List assignedToTaskBoardFormat](../api/plannertask-list-assignedtotaskboardformat.md)|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) collection|Get the plannerAssignedToTaskBoardTaskFormats from the assignedToTaskBoardFormat navigation property.|
|[Create assignedToTaskBoardFormat](../api/plannertask-post-assignedtotaskboardformat.md)|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md)|Create a new assignedToTaskBoardFormat object.|
|[Delete assignedToTaskBoardFormat](../api/plannertask-delete-assignedtotaskboardformat.md)|None|Delete a [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object.|
|[Update assignedToTaskBoardFormat](../api/plannertask-update-assignedtotaskboardformat.md)|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md)|Update the properties of an assignedToTaskBoardFormat object.|
|[Get assignedToTaskBoardFormat](../api/plannertask-get-plannerassignedtotaskboardtaskformat.md)|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md)|Read the properties and relationships of a [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object.|
|[List progressTaskBoardFormat](../api/plannertask-list-progresstaskboardformat.md)|[plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) collection|Get the plannerProgressTaskBoardTaskFormats from the progressTaskBoardFormat navigation property.|
|[Create progressTaskBoardFormat](../api/plannertask-post-progresstaskboardformat.md)|[plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md)|Create a new progressTaskBoardFormat object.|
|[Delete progressTaskBoardFormat](../api/plannertask-delete-progresstaskboardformat.md)|None|Delete a [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object.|
|[Update progressTaskBoardFormat](../api/plannertask-update-progresstaskboardformat.md)|[plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md)|Update the properties of a progressTaskBoardFormat object.|
|[Get progressTaskBoardFormat](../api/plannertask-get-plannerprogresstaskboardtaskformat.md)|[plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md)|Read the properties and relationships of a [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object.|
|[List bucketTaskBoardFormat](../api/plannertask-list-buckettaskboardformat.md)|[plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) collection|Get the plannerBucketTaskBoardTaskFormats from the bucketTaskBoardFormat navigation property.|
|[Create bucketTaskBoardFormat](../api/plannertask-post-buckettaskboardformat.md)|[plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md)|Create a new bucketTaskBoardFormat object.|
|[Delete bucketTaskBoardFormat](../api/plannertask-delete-buckettaskboardformat.md)|None|Delete a [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object.|
|[Update bucketTaskBoardFormat](../api/plannertask-update-buckettaskboardformat.md)|[plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md)|Update the properties of a bucketTaskBoardFormat object.|
|[Get bucketTaskBoardFormat](../api/plannertask-get-plannerbuckettaskboardtaskformat.md)|[plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md)|Read the properties and relationships of a [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeChecklistItemCount|Int32|**TODO: Add Description**|
|appliedCategories|[plannerAppliedCategories](../resources/plannerappliedcategories.md)|**TODO: Add Description**|
|assigneePriority|String|**TODO: Add Description**|
|assignments|[plannerAssignments](../resources/plannerassignments.md)|**TODO: Add Description**|
|bucketId|String|**TODO: Add Description**|
|checklistItemCount|Int32|**TODO: Add Description**|
|completedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|completedDateTime|DateTimeOffset|**TODO: Add Description**|
|conversationThreadId|String|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|dueDateTime|DateTimeOffset|**TODO: Add Description**|
|hasDescription|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|orderHint|String|**TODO: Add Description**|
|percentComplete|Int32|**TODO: Add Description**|
|planId|String|**TODO: Add Description**|
|previewType|plannerPreviewType|**TODO: Add Description**. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.|
|referenceCount|Int32|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|title|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignedToTaskBoardFormat|[plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md)|**TODO: Add Description**|
|bucketTaskBoardFormat|[plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md)|**TODO: Add Description**|
|details|[plannerTaskDetails](../resources/plannertaskdetails.md)|**TODO: Add Description**|
|progressTaskBoardFormat|[plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.plannerTask",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.plannerTask",
  "id": "String (identifier)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "planId": "String",
  "bucketId": "String",
  "title": "String",
  "orderHint": "String",
  "assigneePriority": "String",
  "percentComplete": "Integer",
  "startDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "hasDescription": "Boolean",
  "previewType": "String",
  "completedDateTime": "String (timestamp)",
  "completedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "referenceCount": "Integer",
  "checklistItemCount": "Integer",
  "activeChecklistItemCount": "Integer",
  "appliedCategories": {
    "@odata.type": "microsoft.graph.plannerAppliedCategories"
  },
  "assignments": {
    "@odata.type": "microsoft.graph.plannerAssignments"
  },
  "conversationThreadId": "String"
}
```

