---
title: "Get educationAssignment"
description: "Read properties and relationships of the educationAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get educationAssignment

Namespace: microsoft.graph

Read properties and relationships of the [educationAssignment](../resources/educationassignment.md) object.

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
GET /education/classes/{educationClassId}/assignments/{educationAssignmentId}
GET /education/classes/{educationClassId}/members/{educationUserId}/assignments/{educationAssignmentId}
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
If successful, this method returns a `200 OK` response code and [educationAssignment](../resources/educationassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_educationassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1469

{
  "value": {
    "@odata.type": "#microsoft.graph.educationAssignment",
    "id": "c1883ef5-3ef5-c188-f53e-88c1f53e88c1",
    "classId": "Class Id value",
    "displayName": "Display Name value",
    "instructions": {
      "@odata.type": "microsoft.graph.educationItemBody",
      "contentType": "String",
      "content": "Content value"
    },
    "closeDateTime": "2017-01-01T00:00:08.5448037+00:00",
    "dueDateTime": "2016-12-31T23:56:48.133931+00:00",
    "assignDateTime": "2016-12-31T23:58:31.8700343+00:00",
    "assignedDateTime": "2017-01-01T00:02:08.3128832+00:00",
    "grading": {
      "@odata.type": "microsoft.graph.educationAssignmentGradeType"
    },
    "assignTo": {
      "@odata.type": "microsoft.graph.educationAssignmentRecipient"
    },
    "allowLateSubmissions": true,
    "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "id": "Id value"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "allowStudentsToAddResourcesToSubmission": true,
    "status": "String"
  }
}
```

