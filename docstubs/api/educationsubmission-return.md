---
title: "return"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# return

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
POST /education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}/return
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [educationSubmission](../resources/educationsubmission.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "educationsubmission_return"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}/return
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationsubmission"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 905

{
  "value": {
    "@odata.type": "#microsoft.graph.educationSubmission",
    "id": "5eec38b5-38b5-5eec-b538-ec5eb538ec5e",
    "recipient": {
      "@odata.type": "microsoft.graph.educationSubmissionRecipient"
    },
    "status": "String",
    "submittedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "submittedDateTime": "2017-01-01T00:01:48.6656487+03:00",
    "unsubmittedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "unsubmittedDateTime": "2016-12-31T23:58:19.4345954+03:00",
    "releasedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "releasedDateTime": "2016-12-31T23:57:19.6750904+03:00",
    "returnedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "returnedDateTime": "2017-01-01T00:03:02.7257866+03:00",
    "resourcesFolderUrl": "https://example.com/resourcesFolderUrl/"
  }
}
```

