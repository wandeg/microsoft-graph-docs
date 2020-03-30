---
title: "Get educationSubmissionResource"
description: "Read properties and relationships of the educationSubmissionResource object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get educationSubmissionResource

Namespace: microsoft.graph

Read properties and relationships of the [educationSubmissionResource](../resources/educationsubmissionresource.md) object.

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
GET /education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}/resources/{educationSubmissionResourceId}
GET /education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}/submittedResources/{educationSubmissionResourceId}
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
If successful, this method returns a `200 OK` response code and [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationsubmissionresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}/resources/{educationSubmissionResourceId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 944

{
  "value": {
    "@odata.type": "#microsoft.graph.educationSubmissionResource",
    "id": "a18e50e3-50e3-a18e-e350-8ea1e3508ea1",
    "resource": {
      "@odata.type": "microsoft.graph.educationResource",
      "displayName": "Display Name value",
      "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
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
      "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      }
    },
    "assignmentResourceUrl": "https://example.com/assignmentResourceUrl/"
  }
}
```

