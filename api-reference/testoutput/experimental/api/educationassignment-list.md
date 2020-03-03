---
title: "List educationAssignments"
description: "List properties and relationships of the educationAssignment objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List educationAssignments

Namespace: microsoft.graph

List properties and relationships of the [educationAssignment](../resources/educationassignment.md) objects.

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
GET /education/classes/{educationClassId}/assignments
GET /education/classes/{educationClassId}/members/{educationUserId}/assignments
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationassignment"
}
-->
``` http
GET https://graph.microsoft.com/localtest/education/classes/{educationClassId}/assignments
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationassignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1562

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationAssignment",
      "id": "f3f25053-5053-f3f2-5350-f2f35350f2f3",
      "classId": "Class Id value",
      "displayName": "Display Name value",
      "instructions": {
        "@odata.type": "microsoft.graph.educationItemBody",
        "contentType": "String",
        "content": "Content value"
      },
      "closeDateTime": "2017-01-01T00:01:20.1298622+03:00",
      "dueDateTime": "2017-01-01T00:01:36.4685818+03:00",
      "assignDateTime": "2016-12-31T23:59:28.9197423+03:00",
      "assignedDateTime": "2016-12-31T23:58:09.350506+03:00",
      "grading": {
        "@odata.type": "microsoft.graph.educationAssignmentGradeType"
      },
      "assignTo": {
        "@odata.type": "microsoft.graph.educationAssignmentRecipient"
      },
      "allowLateSubmissions": true,
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
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
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "allowStudentsToAddResourcesToSubmission": true,
      "status": "String"
    }
  ]
}
```

