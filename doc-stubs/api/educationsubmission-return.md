---
title: "educationSubmission: return"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# return

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
POST /education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}/return
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this action returns a `200 OK` response code and a [educationSubmission](../resources/educationsubmission.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}/return
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationsubmission"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.educationSubmission",
    "id": "String (identifier)",
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
}
```

