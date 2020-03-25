---
title: "List tasks"
description: "Get the plannerTasks from the tasks navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List tasks

Namespace: microsoft.graph

Get the plannerTasks from the tasks navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/planner/plans/{plannerPlanId}/buckets/{plannerBucketId}/tasks
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [plannerTask](../resources/plannertask.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_plannertask"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/planner/plans/{plannerPlanId}/buckets/{plannerBucketId}/tasks
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.plannertask)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1557

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.plannerTask",
      "id": "3fc83627-3627-3fc8-2736-c83f2736c83f",
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
      "startDateTime": "2017-01-01T00:01:40.4483143+03:00",
      "createdDateTime": "2017-01-01T00:01:12.6625387+03:00",
      "dueDateTime": "2017-01-01T00:00:25.5677916+03:00",
      "hasDescription": true,
      "previewType": "String",
      "completedDateTime": "2016-12-31T23:58:35.2098078+03:00",
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

