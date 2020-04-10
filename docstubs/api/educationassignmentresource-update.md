---
title: "Update educationAssignmentResource"
description: "Update the properties of a educationAssignmentResource object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update educationAssignmentResource

Namespace: microsoft.graph

Update the properties of a [educationAssignmentResource](../resources/educationassignmentresource.md) object.

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
PATCH /education/classes/{educationClassId}/assignments/{educationAssignmentId}/resources/{educationAssignmentResourceId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [educationAssignmentResource](../resources/educationassignmentresource.md) object.

The following table shows the properties that are required when you create the [educationAssignmentResource](../resources/educationassignmentresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|distributeForStudentWork|Boolean||
|resource|[educationResource](../resources/educationresource.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_educationassignmentresource"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/resources/{educationAssignmentResourceId}
Content-type: application/json
Content-length: 789

{
  "@odata.type": "#microsoft.graph.educationAssignmentResource",
  "distributeForStudentWork": true,
  "resource": {
    "@odata.type": "microsoft.graph.educationResource",
    "displayName": "Display Name value",
    "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
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
    "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    }
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 838

{
  "@odata.type": "#microsoft.graph.educationAssignmentResource",
  "id": "f5f98321-8321-f5f9-2183-f9f52183f9f5",
  "distributeForStudentWork": true,
  "resource": {
    "@odata.type": "microsoft.graph.educationResource",
    "displayName": "Display Name value",
    "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
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
    "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    }
  }
}
```

