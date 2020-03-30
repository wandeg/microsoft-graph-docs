---
title: "Get plannerTask"
description: "Read properties and relationships of the plannerTask object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get plannerTask

Namespace: microsoft.graph

Read properties and relationships of the [plannerTask](../resources/plannertask.md) object.

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
GET /planner/tasks/{plannerTaskId}
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
If successful, this method returns a `200 OK` response code and [plannerTask](../resources/plannertask.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_plannertask"
}
-->
``` http
GET https://graph.microsoft.com/beta/planner/tasks/{plannerTaskId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1480

{
  "value": {
    "@odata.type": "#microsoft.graph.plannerTask",
    "id": "c4c45af4-5af4-c4c4-f45a-c4c4f45ac4c4",
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
    "startDateTime": "2017-01-01T00:02:37.6086584+03:00",
    "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
    "dueDateTime": "2017-01-01T00:03:18.797727+03:00",
    "hasDescription": true,
    "previewType": "String",
    "completedDateTime": "2017-01-01T00:01:28.4865953+03:00",
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
}
```

