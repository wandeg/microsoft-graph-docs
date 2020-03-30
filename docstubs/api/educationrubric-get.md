---
title: "Get educationRubric"
description: "Read properties and relationships of the educationRubric object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get educationRubric

Namespace: microsoft.graph

Read properties and relationships of the [educationRubric](../resources/educationrubric.md) object.

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
GET /education/classes/{educationClassId}/assignments/{educationAssignmentId}/rubric
GET /education/classes/{educationClassId}/members/{educationUserId}/rubrics/{educationRubricId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [educationRubric](../resources/educationrubric.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationrubric"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/rubric
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubric"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1561

{
  "value": {
    "@odata.type": "#microsoft.graph.educationRubric",
    "id": "8e03a794-a794-8e03-94a7-038e94a7038e",
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
  }
}
```

