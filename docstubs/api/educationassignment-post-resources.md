---
title: "Add resources"
description: "Add resources by posting to the resources collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add resources

Namespace: microsoft.graph

Add resources by posting to the resources collection.

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
POST /education/classes/{educationClassId}/assignments/{educationAssignmentId}/resources/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [educationAssignmentResource](../resources/educationassignmentresource.md) object.

The following table shows the properties that are required when you create the [educationAssignmentResource](../resources/educationassignmentresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|distributeForStudentWork|Boolean||
|resource|[educationResource](../resources/educationresource.md)||



## Response
If successful, this method returns a `201 Created` response code and a [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_educationassignmentresource_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/resources
Content-type: application/json
Content-length: 789

{
  "@odata.type": "#microsoft.graph.educationAssignmentResource",
  "distributeForStudentWork": true,
  "resource": {
    "@odata.type": "microsoft.graph.educationResource",
    "displayName": "Display Name value",
    "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
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
    "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    }
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationassignmentresource"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 838

{
  "@odata.type": "#microsoft.graph.educationAssignmentResource",
  "id": "a2788b0b-8b0b-a278-0b8b-78a20b8b78a2",
  "distributeForStudentWork": true,
  "resource": {
    "@odata.type": "microsoft.graph.educationResource",
    "displayName": "Display Name value",
    "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
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
    "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    }
  }
}
```

