---
title: "Get educationAssignmentResource"
description: "Read properties and relationships of the educationAssignmentResource object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get educationAssignmentResource

Namespace: microsoft.graph

Read properties and relationships of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.

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
GET /education/classes/{educationClassId}/assignments/{educationAssignmentId}/resources/{educationAssignmentResourceId}
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
If successful, this method returns a `200 OK` response code and [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationassignmentresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/resources/{educationAssignmentResourceId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 907

{
  "value": {
    "@odata.type": "#microsoft.graph.educationAssignmentResource",
    "id": "9107a71d-a71d-9107-1da7-07911da70791",
    "distributeForStudentWork": true,
    "resource": {
      "@odata.type": "microsoft.graph.educationResource",
      "displayName": "Display Name value",
      "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
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
      "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      }
    }
  }
}
```

