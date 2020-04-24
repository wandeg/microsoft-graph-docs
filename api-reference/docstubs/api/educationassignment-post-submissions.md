---
title: "Create submissions"
description: "Create a new submissions object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create submissions

Namespace: microsoft.graph

Create a new submissions object.

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
POST /education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [educationSubmission](../resources/educationsubmission.md) object.

The following table shows the properties that are required when you create the [educationSubmission](../resources/educationsubmission.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|recipient|[educationSubmissionRecipient](../resources/educationsubmissionrecipient.md)|**TODO: Add Description**|
|status|educationSubmissionStatus|**TODO: Add Description**. Possible values are: `working`, `submitted`, `released`, `returned`, `unknownFutureValue`.|
|submittedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|submittedDateTime|DateTimeOffset|**TODO: Add Description**|
|unsubmittedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|unsubmittedDateTime|DateTimeOffset|**TODO: Add Description**|
|releasedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|releasedDateTime|DateTimeOffset|**TODO: Add Description**|
|returnedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|returnedDateTime|DateTimeOffset|**TODO: Add Description**|
|resourcesFolderUrl|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [educationSubmission](../resources/educationsubmission.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_educationsubmission_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions
Content-Type: application/json
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
HTTP/1.1 201 Created
Content-Type: application/json
{
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
```

