---
title: "Update educationAssignmentResource"
description: "Update the properties of an educationAssignmentResource object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update educationAssignmentResource

Namespace: microsoft.graph

Update the properties of an [educationAssignmentResource](../resources/educationassignmentresource.md) object.

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
PATCH /education/classes/{educationClassId}/assignments/{educationAssignmentId}/resources/{educationAssignmentResourceId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.

The following table shows the properties that are required when you create the [educationAssignmentResource](../resources/educationassignmentresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|distributeForStudentWork|Boolean|**TODO: Add Description**|
|resource|[educationResource](../resources/educationresource.md)|**TODO: Add Description**|



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
Content-Type: application/json
Content-length: 789

{
  "@odata.type": "#microsoft.graph.educationAssignmentResource",
  "distributeForStudentWork": true,
  "resource": {
    "@odata.type": "microsoft.graph.educationResource",
    "displayName": "Display Name value",
    "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
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
    "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    }
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.educationAssignmentResource",
  "id": "3ae40063-0063-3ae4-6300-e43a6300e43a",
  "distributeForStudentWork": true,
  "resource": {
    "@odata.type": "microsoft.graph.educationResource",
    "displayName": "Display Name value",
    "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
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
    "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    }
  }
}
```

