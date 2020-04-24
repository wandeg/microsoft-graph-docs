---
title: "Create rubric"
description: "Create a new rubric object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create rubric

Namespace: microsoft.graph

Create a new rubric object.

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
POST /education/classes/{educationClassId}/assignments/{educationAssignmentId}/rubric
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [educationRubric](../resources/educationrubric.md) object.

The following table shows the properties that are required when you create the [educationRubric](../resources/educationrubric.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|description|[educationItemBody](../resources/educationitembody.md)|**TODO: Add Description**|
|qualities|[rubricQuality](../resources/rubricquality.md) collection|**TODO: Add Description**|
|levels|[rubricLevel](../resources/rubriclevel.md) collection|**TODO: Add Description**|
|grading|[educationAssignmentGradeType](../resources/educationassignmentgradetype.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [educationRubric](../resources/educationrubric.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/rubric
Content-Type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.educationRubric",
  "displayName": "Display Name value",
  "description": {
    "@odata.type": "microsoft.graph.educationItemBody",
    "contentType": "String",
    "content": "Content value"
  },
  "qualities": [
    {
      "@odata.type": "microsoft.graph.rubricQuality",
      "qualityId": "Quality Id value",
      "weight": "Single",
      "criteria": [
        {
          "@odata.type": "microsoft.graph.rubricCriterion"
        }
      ]
    }
  ],
  "levels": [
    {
      "@odata.type": "microsoft.graph.rubricLevel",
      "levelId": "Level Id value",
      "grading": {
        "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": "Single"
      }
    }
  ],
  "grading": {
    "@odata.type": "microsoft.graph.educationAssignmentGradeType"
  },
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
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationrubric"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.educationRubric",
  "id": "ae9a505f-505f-ae9a-5f50-9aae5f509aae",
  "displayName": "Display Name value",
  "description": {
    "@odata.type": "microsoft.graph.educationItemBody",
    "contentType": "String",
    "content": "Content value"
  },
  "qualities": [
    {
      "@odata.type": "microsoft.graph.rubricQuality",
      "qualityId": "Quality Id value",
      "weight": "Single",
      "criteria": [
        {
          "@odata.type": "microsoft.graph.rubricCriterion"
        }
      ]
    }
  ],
  "levels": [
    {
      "@odata.type": "microsoft.graph.rubricLevel",
      "levelId": "Level Id value",
      "grading": {
        "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType",
        "maxPoints": "Single"
      }
    }
  ],
  "grading": {
    "@odata.type": "microsoft.graph.educationAssignmentGradeType"
  },
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
```

