---
title: "List educationSubmissions"
description: "List properties and relationships of the educationSubmission objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List educationSubmissions

Namespace: microsoft.graph

List properties and relationships of the [educationSubmission](../resources/educationsubmission.md) objects.

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
GET /education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationsubmission"
}
-->
``` http
GET https://graph.microsoft.com/localtest/education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationsubmission)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1303

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationSubmission",
      "id": "00b163fd-63fd-00b1-fd63-b100fd63b100",
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
      "submittedDateTime": "2016-12-31T23:57:10.5476387+03:00",
      "unsubmittedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "unsubmittedDateTime": "2017-01-01T00:02:16.2566523+03:00",
      "releasedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "releasedDateTime": "2016-12-31T23:59:18.4243169+03:00",
      "returnedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "returnedDateTime": "2017-01-01T00:00:10.2935801+03:00",
      "resourcesFolderUrl": "https://example.com/resourcesFolderUrl/"
    }
  ]
}
```

