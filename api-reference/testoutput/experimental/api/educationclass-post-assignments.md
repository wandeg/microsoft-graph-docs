---
title: "Add assignments"
description: "Add assignments by posting to the assignments collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add assignments

Add assignments by posting to the assignments collection.

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
POST /education/classes/{educationClassId}/assignments/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the educationAssignment object.

The following table shows the properties that are required when you create the educationAssignment.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|classId|String||
|displayName|String||
|instructions|[educationItemBody](../resources/educationItemBody.md)||
|closeDateTime|DateTimeOffset||
|dueDateTime|DateTimeOffset||
|assignDateTime|DateTimeOffset||
|assignedDateTime|DateTimeOffset||
|grading|[educationAssignmentGradeType](../resources/educationAssignmentGradeType.md)||
|assignTo|[educationAssignmentRecipient](../resources/educationAssignmentRecipient.md)||
|allowLateSubmissions|Boolean||
|createdDateTime|DateTimeOffset||
|createdBy|[identitySet](../resources/identitySet.md)||
|lastModifiedDateTime|DateTimeOffset||
|lastModifiedBy|[identitySet](../resources/identitySet.md)||
|allowStudentsToAddResourcesToSubmission|Boolean||
|status|Enumeration|. Possible values are: `draft`, `published`, `assigned`, `unknownFutureValue`.|



## Response
If successful, this method returns a `201 Created` response code and a [educationAssignment](../resources/educationassignment.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_educationassignment_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/education/classes/{educationClassId}/assignments
Content-type: application/json
Content-length: 1120

{
  "@odata.type": "#microsoft.graph.educationAssignment",
  "classId": "Class Id value",
  "displayName": "Display Name value",
  "instructions": {
    "@odata.type": "microsoft.graph.educationItemBody",
    "contentType": "String",
    "content": "Content value"
  },
  "closeDateTime": "2016-12-31T23:56:24.9256365+03:00",
  "dueDateTime": "2016-12-31T23:57:44.4001585+03:00",
  "assignDateTime": "2017-01-01T00:01:55.1489412+03:00",
  "assignedDateTime": "2017-01-01T00:00:28.0288253+03:00",
  "grading": {
    "@odata.type": "microsoft.graph.educationAssignmentGradeType"
  },
  "assignTo": {
    "@odata.type": "microsoft.graph.educationAssignmentRecipient"
  },
  "allowLateSubmissions": true,
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
  "allowStudentsToAddResourcesToSubmission": true,
  "status": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1371

{
  "@odata.type": "#microsoft.graph.educationAssignment",
  "id": "7e577ae4-7ae4-7e57-e47a-577ee47a577e",
  "classId": "Class Id value",
  "displayName": "Display Name value",
  "instructions": {
    "@odata.type": "microsoft.graph.educationItemBody",
    "contentType": "String",
    "content": "Content value"
  },
  "closeDateTime": "2016-12-31T23:56:24.9256365+03:00",
  "dueDateTime": "2016-12-31T23:57:44.4001585+03:00",
  "assignDateTime": "2017-01-01T00:01:55.1489412+03:00",
  "assignedDateTime": "2017-01-01T00:00:28.0288253+03:00",
  "grading": {
    "@odata.type": "microsoft.graph.educationAssignmentGradeType"
  },
  "assignTo": {
    "@odata.type": "microsoft.graph.educationAssignmentRecipient"
  },
  "allowLateSubmissions": true,
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
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
  "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "allowStudentsToAddResourcesToSubmission": true,
  "status": "String"
}
```

