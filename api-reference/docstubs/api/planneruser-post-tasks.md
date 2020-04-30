---
title: "Add tasks"
description: "Add tasks by posting to the tasks collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add tasks

Namespace: microsoft.graph

Add tasks by posting to the tasks collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/planner/tasks/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [plannerTask](../resources/plannertask.md) object.

The following table shows the properties that are required when you create the [plannerTask](../resources/plannertask.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|planId|String|**TODO: Add Description**|
|bucketId|String|**TODO: Add Description**|
|title|String|**TODO: Add Description**|
|orderHint|String|**TODO: Add Description**|
|assigneePriority|String|**TODO: Add Description**|
|percentComplete|Int32|**TODO: Add Description**|
|priority|Int32|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|dueDateTime|DateTimeOffset|**TODO: Add Description**|
|hasDescription|Boolean|**TODO: Add Description**|
|previewType|plannerPreviewType|**TODO: Add Description**. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.|
|completedDateTime|DateTimeOffset|**TODO: Add Description**|
|completedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|referenceCount|Int32|**TODO: Add Description**|
|checklistItemCount|Int32|**TODO: Add Description**|
|activeChecklistItemCount|Int32|**TODO: Add Description**|
|appliedCategories|[plannerAppliedCategories](../resources/plannerappliedcategories.md)|**TODO: Add Description**|
|assignments|[plannerAssignments](../resources/plannerassignments.md)|**TODO: Add Description**|
|conversationThreadId|String|**TODO: Add Description**|



## Response
If successful, this method returns a `204 No Content` response code and a [plannerTask](../resources/plannertask.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_plannertask_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/planner/tasks/$ref
Content-Type: application/json
Content-length: 904

{
  "@odata.type": "#microsoft.graph.plannerTask",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "planId": "String",
  "bucketId": "String",
  "title": "String",
  "orderHint": "String",
  "assigneePriority": "String",
  "percentComplete": "Integer",
  "priority": "Integer",
  "startDateTime": "String (timestamp)",
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

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannertask"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.plannerTask",
  "id": "3fa468c2-68c2-3fa4-c268-a43fc268a43f",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "planId": "String",
  "bucketId": "String",
  "title": "String",
  "orderHint": "String",
  "assigneePriority": "String",
  "percentComplete": "Integer",
  "priority": "Integer",
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

