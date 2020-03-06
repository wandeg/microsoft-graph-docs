---
title: "Add submissions"
description: "Add submissions by posting to the submissions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add submissions

Namespace: microsoft.graph

Add submissions by posting to the submissions collection.

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
POST /education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [educationSubmission](../resources/educationsubmission.md) object.

The following table shows the properties that are required when you create the [educationSubmission](../resources/educationsubmission.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|recipient|[educationSubmissionRecipient](../resources/educationsubmissionrecipient.md)||
|status|Enumeration|. Possible values are: `working`, `submitted`, `released`, `returned`, `unknownFutureValue`.|
|submittedBy|[identitySet](../resources/identityset.md)||
|submittedDateTime|DateTimeOffset||
|unsubmittedBy|[identitySet](../resources/identityset.md)||
|unsubmittedDateTime|DateTimeOffset||
|releasedBy|[identitySet](../resources/identityset.md)||
|releasedDateTime|DateTimeOffset||
|returnedBy|[identitySet](../resources/identityset.md)||
|returnedDateTime|DateTimeOffset||
|resourcesFolderUrl|String||



## Response
If successful, this method returns a `201 Created` response code and a [educationSubmission](../resources/educationsubmission.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_educationsubmission_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions
Content-type: application/json
Content-length: 1085

{
  "@odata.type": "#microsoft.graph.educationSubmission",
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
  "submittedDateTime": "2016-12-31T23:56:39.8413838+03:00",
  "unsubmittedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "unsubmittedDateTime": "2017-01-01T00:01:37.8870443+03:00",
  "releasedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "releasedDateTime": "2017-01-01T00:00:01.1001695+03:00",
  "returnedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "returnedDateTime": "2016-12-31T23:57:07.5874584+03:00",
  "resourcesFolderUrl": "https://example.com/resourcesFolderUrl/"
}
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1134

{
  "@odata.type": "#microsoft.graph.educationSubmission",
  "id": "0e834e62-4e62-0e83-624e-830e624e830e",
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
  "submittedDateTime": "2016-12-31T23:56:39.8413838+03:00",
  "unsubmittedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "unsubmittedDateTime": "2017-01-01T00:01:37.8870443+03:00",
  "releasedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "releasedDateTime": "2017-01-01T00:00:01.1001695+03:00",
  "returnedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "returnedDateTime": "2016-12-31T23:57:07.5874584+03:00",
  "resourcesFolderUrl": "https://example.com/resourcesFolderUrl/"
}
```

