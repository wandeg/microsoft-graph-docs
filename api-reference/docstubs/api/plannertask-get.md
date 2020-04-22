---
title: "Get plannerTask"
description: "Read properties and relationships of a plannerTask object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get plannerTask

Namespace: microsoft.graph

Read properties and relationships of a [plannerTask](../resources/plannertask.md) object.

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
GET /planner/tasks/{plannerTaskId}
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
If successful, this method returns a `200 OK` response code and a [plannerTask](../resources/plannertask.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_plannertask"
}
-->
``` http
GET https://graph.microsoft.com/beta/planner/tasks/{plannerTaskId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
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
}
```

