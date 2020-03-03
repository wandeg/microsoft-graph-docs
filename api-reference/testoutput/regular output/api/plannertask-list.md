---
title: "List plannerTasks"
description: "List properties and relationships of the plannerTask objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List plannerTasks

Namespace: microsoft.graph

List properties and relationships of the [plannerTask](../resources/plannertask.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /planner/tasks
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [plannerTask](../resources/plannertask.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_plannertask"
}
-->
``` http
GET https://graph.microsoft.com/localtest/planner/tasks
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
Content-Length: 1556

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.plannerTask",
      "id": "eaa76e14-6e14-eaa7-146e-a7ea146ea7ea",
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
      "startDateTime": "2016-12-31T23:59:14.2230899+03:00",
      "createdDateTime": "2017-01-01T00:02:24.618735+03:00",
      "dueDateTime": "2017-01-01T00:00:08.6678478+03:00",
      "hasDescription": true,
      "previewType": "String",
      "completedDateTime": "2017-01-01T00:03:28.7389204+03:00",
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

