---
title: "Add rubrics"
description: "Add rubrics by posting to the rubrics collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add rubrics

Namespace: microsoft.graph

Add rubrics by posting to the rubrics collection.

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
POST /education/classes/{educationClassId}/members/{educationUserId}/rubrics/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [educationRubric](../resources/educationrubric.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_educationrubric_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/members/{educationUserId}/rubrics
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
  "id": "615f9b2c-9b2c-615f-2c9b-5f612c9b5f61",
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
```

