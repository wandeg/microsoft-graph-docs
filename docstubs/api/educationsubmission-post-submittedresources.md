---
title: "Add submittedResources"
description: "Add submittedResources by posting to the submittedResources collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add submittedResources

Namespace: microsoft.graph

Add submittedResources by posting to the submittedResources collection.

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
POST /education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}/submittedResources/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [educationSubmissionResource](../resources/educationsubmissionresource.md) object.

The following table shows the properties that are required when you create the [educationSubmissionResource](../resources/educationsubmissionresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|resource|[educationResource](../resources/educationresource.md)||
|assignmentResourceUrl|String||



## Response
If successful, this method returns a `201 Created` response code and a [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_educationsubmissionresource_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}/submittedResources
Content-type: application/json
Content-length: 826

{
  "@odata.type": "#microsoft.graph.educationSubmissionResource",
  "resource": {
    "@odata.type": "microsoft.graph.educationResource",
    "displayName": "Display Name value",
    "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "id": "Id value"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    }
  },
  "assignmentResourceUrl": "https://example.com/assignmentResourceUrl/"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationsubmissionresource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 875

{
  "@odata.type": "#microsoft.graph.educationSubmissionResource",
  "id": "4b62440c-440c-4b62-0c44-624b0c44624b",
  "resource": {
    "@odata.type": "microsoft.graph.educationResource",
    "displayName": "Display Name value",
    "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "id": "Id value"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    }
  },
  "assignmentResourceUrl": "https://example.com/assignmentResourceUrl/"
}
```

