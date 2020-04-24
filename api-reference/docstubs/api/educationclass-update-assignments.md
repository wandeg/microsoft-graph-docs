---
title: "Update assignments"
description: "Update the properties of an assignments object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update assignments

Namespace: microsoft.graph

Update the properties of an assignments object.

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
PATCH /education/classes/{educationClassId}/assignments
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [educationAssignment](../resources/educationassignment.md) object.

The following table shows the properties that are required when you create the [educationAssignment](../resources/educationassignment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|classId|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|instructions|[educationItemBody](../resources/educationitembody.md)|**TODO: Add Description**|
|closeDateTime|DateTimeOffset|**TODO: Add Description**|
|dueDateTime|DateTimeOffset|**TODO: Add Description**|
|assignDateTime|DateTimeOffset|**TODO: Add Description**|
|assignedDateTime|DateTimeOffset|**TODO: Add Description**|
|grading|[educationAssignmentGradeType](../resources/educationassignmentgradetype.md)|**TODO: Add Description**|
|assignTo|[educationAssignmentRecipient](../resources/educationassignmentrecipient.md)|**TODO: Add Description**|
|allowLateSubmissions|Boolean|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|allowStudentsToAddResourcesToSubmission|Boolean|**TODO: Add Description**|
|status|educationAssignmentStatus|**TODO: Add Description**. Possible values are: `draft`, `published`, `assigned`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [educationAssignment](../resources/educationassignment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_assignments"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments
Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
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
```

