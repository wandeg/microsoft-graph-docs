---
title: "Update educationSubmission"
description: "Update the properties of a educationSubmission object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update educationSubmission

Namespace: microsoft.graph

Update the properties of a [educationSubmission](../resources/educationsubmission.md) object.

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
PATCH /education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [educationSubmission](../resources/educationsubmission.md) object.

The following table shows the properties that are required when you create the [educationSubmission](../resources/educationsubmission.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|recipient|[educationSubmissionRecipient](../resources/educationsubmissionrecipient.md)||
|status|Enumeration| Possible values are: `working`, `submitted`, `released`, `returned`, `unknownFutureValue`.|
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
If successful, this method returns a `200 OK` response code and an updated [educationSubmission](../resources/educationsubmission.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_educationsubmission"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}
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
  "submittedDateTime": "2017-01-01T00:00:52.4799349+03:00",
  "unsubmittedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "unsubmittedDateTime": "2016-12-31T23:58:28.4121968+03:00",
  "releasedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "releasedDateTime": "2017-01-01T00:02:01.4226305+03:00",
  "returnedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "returnedDateTime": "2016-12-31T23:57:14.0344387+03:00",
  "resourcesFolderUrl": "https://example.com/resourcesFolderUrl/"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1134

{
  "@odata.type": "#microsoft.graph.educationSubmission",
  "id": "908ef6e1-f6e1-908e-e1f6-8e90e1f68e90",
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
  "submittedDateTime": "2017-01-01T00:00:52.4799349+03:00",
  "unsubmittedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "unsubmittedDateTime": "2016-12-31T23:58:28.4121968+03:00",
  "releasedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "releasedDateTime": "2017-01-01T00:02:01.4226305+03:00",
  "returnedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "returnedDateTime": "2016-12-31T23:57:14.0344387+03:00",
  "resourcesFolderUrl": "https://example.com/resourcesFolderUrl/"
}
```

