---
title: "List assignments"
description: "Get the educationAssignments from the assignments navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List assignments

Namespace: microsoft.graph

Get the educationAssignments from the assignments navigation property.

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
GET /education/classes/{educationClassId}/assignments
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
If successful, this method returns a `200 OK` response code and a collection of [educationAssignment](../resources/educationassignment.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_educationassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationassignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationAssignment",
      "id": "49cd9cb4-9cb4-49cd-b49c-cd49b49ccd49",
      "classId": "Class Id value",
      "displayName": "Display Name value",
      "instructions": {
        "@odata.type": "microsoft.graph.educationItemBody",
        "contentType": "String",
        "content": "Content value"
      },
      "closeDateTime": "2017-01-01T00:00:08.6183578+03:00",
      "dueDateTime": "2017-01-01T00:03:16.4480136+03:00",
      "assignDateTime": "2017-01-01T00:03:30.0658561+03:00",
      "assignedDateTime": "2016-12-31T23:56:57.6905634+03:00",
      "grading": {
        "@odata.type": "microsoft.graph.educationAssignmentGradeType"
      },
      "assignTo": {
        "@odata.type": "microsoft.graph.educationAssignmentRecipient"
      },
      "allowLateSubmissions": true,
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
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
      "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "allowStudentsToAddResourcesToSubmission": true,
      "status": "String"
    }
  ]
}
```

