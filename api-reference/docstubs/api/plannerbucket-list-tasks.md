---
title: "List tasks"
description: "Get the plannerTasks from the tasks navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List tasks

Namespace: microsoft.graph

Get the plannerTasks from the tasks navigation property.

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
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/planner/plans/{plannerPlanId}/buckets/{plannerBucketId}/tasks
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [plannerTask](../resources/plannertask.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_plannertask"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/planner/plans/{plannerPlanId}/buckets/{plannerBucketId}/tasks
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.plannertask)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.plannerTask",
      "id": "71c61928-1928-71c6-2819-c6712819c671",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet",
        "application": {
          "@odata.type": "microsoft.graph.identity",
          "id": "Id value",
          "displayName": "Display Name value"
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
      "priority": 8,
      "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
      "dueDateTime": "2017-01-01T00:03:16.4480136+03:00",
      "hasDescription": true,
      "previewType": "String",
      "completedDateTime": "2017-01-01T00:02:03.9770517+03:00",
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
  ]
}
```

