---
title: "Update educationRubric"
description: "Update the properties of a educationRubric object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update educationRubric

Namespace: microsoft.graph

Update the properties of a [educationRubric](../resources/educationrubric.md) object.

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
PATCH /education/classes/{educationClassId}/assignments/{educationAssignmentId}/rubric
PATCH /education/classes/{educationClassId}/members/{educationUserId}/rubrics/{educationRubricId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [educationRubric](../resources/educationrubric.md) object.

The following table shows the properties that are required when you create the [educationRubric](../resources/educationrubric.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|[educationItemBody](../resources/educationitembody.md)||
|qualities|[rubricQuality](../resources/rubricquality.md) collection||
|levels|[rubricLevel](../resources/rubriclevel.md) collection||
|grading|[educationAssignmentGradeType](../resources/educationassignmentgradetype.md)||
|createdDateTime|DateTimeOffset||
|createdBy|[identitySet](../resources/identityset.md)||
|lastModifiedDateTime|DateTimeOffset||
|lastModifiedBy|[identitySet](../resources/identityset.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [educationRubric](../resources/educationrubric.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_educationrubric"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/education/classes/{educationClassId}/assignments/{educationAssignmentId}/rubric
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1439

{
  "@odata.type": "#microsoft.graph.educationRubric",
  "id": "f0c2bb23-bb23-f0c2-23bb-c2f023bbc2f0",
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
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
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
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

