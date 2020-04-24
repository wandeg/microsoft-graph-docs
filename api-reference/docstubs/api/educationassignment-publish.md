---
title: "educationAssignment: publish"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# publish

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /education/classes/{educationClassId}/assignments/{educationAssignmentId}/publish
POST /education/classes/{educationClassId}/members/{educationUserId}/assignments/{educationAssignmentId}/publish
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [educationAssignment](../resources/educationassignment.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/publish
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationassignment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.educationAssignment",
    "id": "49cd9cb4-9cb4-49cd-b49c-cd49b49ccd49",
    "classId": "Class Id value",
    "displayName": "Display Name value",
    "instructions": {
      "@odata.type": "microsoft.graph.educationItemBody"
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
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "allowStudentsToAddResourcesToSubmission": true,
    "status": "String"
  }
}
```

