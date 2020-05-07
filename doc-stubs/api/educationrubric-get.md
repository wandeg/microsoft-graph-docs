---
title: "Get educationRubric"
description: "Read the properties and relationships of an educationRubric object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get educationRubric

Namespace: microsoft.graph

Read the properties and relationships of an [educationRubric](../resources/educationrubric.md) object.

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
GET /education/classes/{educationClassId}/assignments/{educationAssignmentId}/rubric
GET /education/classes/{educationClassId}/members/{educationUserId}/rubrics/{educationRubricId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [educationRubric](../resources/educationrubric.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_educationrubric"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/rubric
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.educationRubric",
    "id": "549d55df-55df-549d-df55-9d54df559d54",
    "displayName": "String",
    "description": {
      "@odata.type": "microsoft.graph.educationItemBody"
    },
    "qualities": [
      {
        "@odata.type": "microsoft.graph.rubricQuality"
      }
    ],
    "levels": [
      {
        "@odata.type": "microsoft.graph.rubricLevel"
      }
    ],
    "grading": {
      "@odata.type": "microsoft.graph.educationAssignmentGradeType"
    },
    "createdDateTime": "String (timestamp)",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "String (timestamp)",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    }
  }
}
```

