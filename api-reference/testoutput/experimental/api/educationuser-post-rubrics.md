---
title: "Add rubrics"
description: "Add rubrics by posting to the rubrics collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add rubrics

Add rubrics by posting to the rubrics collection.

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
POST /education/classes/{educationClassId}/members/{educationUserId}/rubrics/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the educationRubric object.

The following table shows the properties that are required when you create the educationRubric.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String||
|description|[educationItemBody](../resources/educationItemBody.md)||
|qualities|[rubricQuality](../resources/rubricQuality.md) collection||
|levels|[rubricLevel](../resources/rubricLevel.md) collection||
|grading|[educationAssignmentGradeType](../resources/educationAssignmentGradeType.md)||
|createdDateTime|DateTimeOffset||
|createdBy|[identitySet](../resources/identitySet.md)||
|lastModifiedDateTime|DateTimeOffset||
|lastModifiedBy|[identitySet](../resources/identitySet.md)||



## Response
If successful, this method returns a `201 Created` response code and a [educationRubric](../resources/educationrubric.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/education/classes/{educationClassId}/members/{educationUserId}/rubrics
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
  "truncated": true,
  "@odata.type": "microsoft.graph.educationrubric"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1440

{
  "@odata.type": "#microsoft.graph.educationRubric",
  "id": "8c75019d-019d-8c75-9d01-758c9d01758c",
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
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
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
  "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

