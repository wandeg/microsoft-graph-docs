---
title: "List submissions"
description: "Get the educationSubmissions from the submissions navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List submissions

Namespace: microsoft.graph

Get the educationSubmissions from the submissions navigation property.

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
GET /education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions
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
If successful, this method returns a `200 OK` response code and a collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationsubmission"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions
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
      "id": "c4f5d02b-d02b-c4f5-2bd0-f5c42bd0f5c4",
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
      "submittedDateTime": "2017-01-01T00:01:19.2814111+00:00",
      "unsubmittedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "unsubmittedDateTime": "2017-01-01T00:02:50.7310383+00:00",
      "releasedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "releasedDateTime": "2017-01-01T00:03:00.5538796+00:00",
      "returnedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "returnedDateTime": "2017-01-01T00:01:18.2057844+00:00",
      "resourcesFolderUrl": "https://example.com/resourcesFolderUrl/"
    }
  ]
}
```

