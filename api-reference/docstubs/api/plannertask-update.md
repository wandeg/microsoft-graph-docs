---
title: "Update plannerTask"
description: "Update the properties of a plannerTask object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update plannerTask

Namespace: microsoft.graph

Update the properties of a [plannerTask](../resources/plannertask.md) object.

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
PATCH /planner/tasks/{plannerTaskId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [plannerTask](../resources/plannertask.md) object.

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
If successful, this method returns a `200 OK` response code and an updated [plannerTask](../resources/plannertask.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_plannertask"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/planner/tasks/{plannerTaskId}
Content-Type: application/json
Content-length: 1252

{
  "@odata.type": "#microsoft.graph.plannerTask",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "Display Name value",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "planId": "Plan Id value",
  "bucketId": "Bucket Id value",
  "title": "Title value",
  "orderHint": "Order Hint value",
  "assigneePriority": "Assignee Priority value",
  "percentComplete": 15,
  "startDateTime": "2016-12-31T23:57:25.6506614+00:00",
  "dueDateTime": "2016-12-31T23:59:46.8308187+00:00",
  "hasDescription": true,
  "previewType": "String",
  "completedDateTime": "2016-12-31T23:57:52.0324439+00:00",
  "completedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "referenceCount": 14,
  "checklistItemCount": 2,
  "activeChecklistItemCount": 8,
  "appliedCategories": {
    "@odata.type": "microsoft.graph.plannerAppliedCategories"
  },
  "assignments": {
    "@odata.type": "microsoft.graph.plannerAssignments"
  },
  "conversationThreadId": "Conversation Thread Id value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.plannerTask",
  "id": "70dcb6db-b6db-70dc-dbb6-dc70dbb6dc70",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "Display Name value",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "planId": "Plan Id value",
  "bucketId": "Bucket Id value",
  "title": "Title value",
  "orderHint": "Order Hint value",
  "assigneePriority": "Assignee Priority value",
  "percentComplete": 15,
  "startDateTime": "2016-12-31T23:57:25.6506614+00:00",
  "createdDateTime": "2017-01-01T00:02:14.13292+00:00",
  "dueDateTime": "2016-12-31T23:59:46.8308187+00:00",
  "hasDescription": true,
  "previewType": "String",
  "completedDateTime": "2016-12-31T23:57:52.0324439+00:00",
  "completedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "referenceCount": 14,
  "checklistItemCount": 2,
  "activeChecklistItemCount": 8,
  "appliedCategories": {
    "@odata.type": "microsoft.graph.plannerAppliedCategories"
  },
  "assignments": {
    "@odata.type": "microsoft.graph.plannerAssignments"
  },
  "conversationThreadId": "Conversation Thread Id value"
}
```

