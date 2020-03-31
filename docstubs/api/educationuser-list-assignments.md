---
title: "List assignments"
description: "Get the educationAssignments from the assignments navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List assignments

Namespace: microsoft.graph

Get the educationAssignments from the assignments navigation property.

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
GET /education/classes/{educationClassId}/members/{educationUserId}/assignments
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
If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{educationClassId}/members/{educationUserId}/assignments
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
Content-Length: 1563

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationAssignment",
      "id": "de8bd984-d984-de8b-84d9-8bde84d98bde",
      "classId": "Class Id value",
      "displayName": "Display Name value",
      "instructions": {
        "@odata.type": "microsoft.graph.educationItemBody",
        "contentType": "String",
        "content": "Content value"
      },
      "closeDateTime": "2017-01-01T00:02:35.7603558+03:00",
      "dueDateTime": "2016-12-31T23:58:49.4995243+03:00",
      "assignDateTime": "2017-01-01T00:01:53.7947334+03:00",
      "assignedDateTime": "2017-01-01T00:00:15.9351772+03:00",
      "grading": {
        "@odata.type": "microsoft.graph.educationAssignmentGradeType"
      },
      "assignTo": {
        "@odata.type": "microsoft.graph.educationAssignmentRecipient"
      },
      "allowLateSubmissions": true,
      "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
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
      "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "allowStudentsToAddResourcesToSubmission": true,
      "status": "String"
    }
  ]
}
```

