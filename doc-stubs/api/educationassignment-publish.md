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
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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
    "id": "String (identifier)",
    "classId": "String",
    "displayName": "String",
    "instructions": {
      "@odata.type": "microsoft.graph.educationItemBody"
    },
    "closeDateTime": "String (timestamp)",
    "dueDateTime": "String (timestamp)",
    "assignDateTime": "String (timestamp)",
    "assignedDateTime": "String (timestamp)",
    "grading": {
      "@odata.type": "microsoft.graph.educationAssignmentGradeType"
    },
    "assignTo": {
      "@odata.type": "microsoft.graph.educationAssignmentRecipient"
    },
    "allowLateSubmissions": "Boolean",
    "createdDateTime": "String (timestamp)",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "String (timestamp)",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "allowStudentsToAddResourcesToSubmission": "Boolean",
    "status": "String"
  }
}
```

