---
title: "Add assignments"
description: "Add assignments by posting to the assignments collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add assignments

Namespace: microsoft.graph

Add assignments by posting to the assignments collection.

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
POST /education/classes/{educationClassId}/assignments/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [educationAssignment](../resources/educationassignment.md) object.

The following table shows the properties that are required when you create the [educationAssignment](../resources/educationassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|classId|String||
|displayName|String||
|instructions|[educationItemBody](../resources/educationitembody.md)||
|closeDateTime|DateTimeOffset||
|dueDateTime|DateTimeOffset||
|assignDateTime|DateTimeOffset||
|assignedDateTime|DateTimeOffset||
|grading|[educationAssignmentGradeType](../resources/educationassignmentgradetype.md)||
|assignTo|[educationAssignmentRecipient](../resources/educationassignmentrecipient.md)||
|allowLateSubmissions|Boolean||
|createdDateTime|DateTimeOffset||
|createdBy|[identitySet](../resources/identityset.md)||
|lastModifiedDateTime|DateTimeOffset||
|lastModifiedBy|[identitySet](../resources/identityset.md)||
|allowStudentsToAddResourcesToSubmission|Boolean||
|status|Enumeration| Possible values are: `draft`, `published`, `assigned`, `unknownFutureValue`.|



## Response
If successful, this method returns a `201 Created` response code and a [educationAssignment](../resources/educationassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_educationassignment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments
Content-type: application/json
Content-length: 1119

{
  "@odata.type": "#microsoft.graph.educationAssignment",
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationassignment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1370

{
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
```

