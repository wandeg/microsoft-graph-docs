---
title: "Add submissions"
description: "Add submissions by posting to the submissions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add submissions

Add submissions by posting to the submissions collection.

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
POST /education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the educationSubmission object.

The following table shows the properties that are required when you create the educationSubmission.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|recipient|[educationSubmissionRecipient](../resources/educationSubmissionRecipient.md)||
|status|Enumeration|. Possible values are: `working`, `submitted`, `released`, `returned`, `unknownFutureValue`.|
|submittedBy|[identitySet](../resources/identitySet.md)||
|submittedDateTime|DateTimeOffset||
|unsubmittedBy|[identitySet](../resources/identitySet.md)||
|unsubmittedDateTime|DateTimeOffset||
|releasedBy|[identitySet](../resources/identitySet.md)||
|releasedDateTime|DateTimeOffset||
|returnedBy|[identitySet](../resources/identitySet.md)||
|returnedDateTime|DateTimeOffset||
|resourcesFolderUrl|String||



## Response
If successful, this method returns a `201 Created` response code and a [educationSubmission](../resources/educationsubmission.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_educationsubmission_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions
Content-type: application/json
Content-length: 1083

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
  "submittedDateTime": "2017-01-01T00:01:39.273323+03:00",
  "unsubmittedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "unsubmittedDateTime": "2016-12-31T23:59:22.7332157+03:00",
  "releasedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "releasedDateTime": "2016-12-31T23:57:12.1158417+03:00",
  "returnedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "returnedDateTime": "2017-01-01T00:02:03.032537+03:00",
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
Content-Length: 1132

{
  "@odata.type": "#microsoft.graph.educationSubmission",
  "id": "f76dfaae-faae-f76d-aefa-6df7aefa6df7",
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
  "submittedDateTime": "2017-01-01T00:01:39.273323+03:00",
  "unsubmittedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "unsubmittedDateTime": "2016-12-31T23:59:22.7332157+03:00",
  "releasedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "releasedDateTime": "2016-12-31T23:57:12.1158417+03:00",
  "returnedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "returnedDateTime": "2017-01-01T00:02:03.032537+03:00",
  "resourcesFolderUrl": "https://example.com/resourcesFolderUrl/"
}
```

