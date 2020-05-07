---
title: "List submissions"
description: "Get the educationSubmissions from the submissions navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List submissions

Namespace: microsoft.graph

Get the educationSubmissions from the submissions navigation property.

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
GET /education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_educationsubmission"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationsubmission)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationSubmission",
      "id": "df692b10-2b10-df69-102b-69df102b69df",
      "recipient": {
        "@odata.type": "microsoft.graph.educationSubmissionRecipient"
      },
      "status": "String",
      "submittedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "submittedDateTime": "String (timestamp)",
      "unsubmittedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "unsubmittedDateTime": "String (timestamp)",
      "releasedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "releasedDateTime": "String (timestamp)",
      "returnedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "returnedDateTime": "String (timestamp)",
      "resourcesFolderUrl": "String"
    }
  ]
}
```

