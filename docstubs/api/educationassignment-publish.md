---
title: "publish"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# publish

Namespace: microsoft.graph



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
POST /education/classes/{educationClassId}/assignments/{educationAssignmentId}/publish
POST /education/classes/{educationClassId}/members/{educationUserId}/assignments/{educationAssignmentId}/publish
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [educationAssignment](../resources/educationassignment.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "educationassignment_publish"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/publish
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
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1133

{
  "value": {
    "@odata.type": "#microsoft.graph.educationAssignment",
    "id": "6f89f6b4-f6b4-6f89-b4f6-896fb4f6896f",
    "classId": "Class Id value",
    "displayName": "Display Name value",
    "instructions": {
      "@odata.type": "microsoft.graph.educationItemBody"
    },
    "closeDateTime": "2016-12-31T23:57:33.5639943+00:00",
    "dueDateTime": "2016-12-31T23:57:05.7334116+00:00",
    "assignDateTime": "2017-01-01T00:00:05.4911878+00:00",
    "assignedDateTime": "2016-12-31T23:56:51.0662343+00:00",
    "grading": {
      "@odata.type": "microsoft.graph.educationAssignmentGradeType"
    },
    "assignTo": {
      "@odata.type": "microsoft.graph.educationAssignmentRecipient"
    },
    "allowLateSubmissions": true,
    "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "allowStudentsToAddResourcesToSubmission": true,
    "status": "String"
  }
}
```

