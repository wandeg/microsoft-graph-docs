---
title: "Get educationSubmission"
description: "Read the properties and relationships of an educationSubmission object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get educationSubmission

Namespace: microsoft.graph

Read the properties and relationships of an [educationSubmission](../resources/educationsubmission.md) object.

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
GET /education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}
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
If successful, this method returns a `200 OK` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_educationsubmission"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.educationSubmission",
    "id": "e8b66d5a-6d5a-e8b6-5a6d-b6e85a6db6e8",
    "recipient": {
      "@odata.type": "microsoft.graph.educationSubmissionRecipient"
    },
    "status": "String",
    "submittedBy": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "id": "Id value",
        "displayName": "Display Name value"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "submittedDateTime": "2017-01-01T00:03:16.4748996+03:00",
    "unsubmittedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "unsubmittedDateTime": "2016-12-31T23:59:16.1194969+03:00",
    "releasedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "releasedDateTime": "2017-01-01T00:02:44.7268822+03:00",
    "returnedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "returnedDateTime": "2017-01-01T00:01:02.2304868+03:00",
    "resourcesFolderUrl": "https://example.com/resourcesFolderUrl/"
  }
}
```

