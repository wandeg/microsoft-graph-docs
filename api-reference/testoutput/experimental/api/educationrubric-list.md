---
title: "List educationRubrics"
description: "List properties and relationships of the educationRubric objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List educationRubrics

Namespace: microsoft.graph

List properties and relationships of the [educationRubric](../resources/educationrubric.md) objects.

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
GET /education/classes/{educationClassId}/members/{educationUserId}/rubrics
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [educationRubric](../resources/educationrubric.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationrubric"
}
-->
``` http
GET https://graph.microsoft.com/localtest/education/classes/{educationClassId}/members/{educationUserId}/rubrics
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationrubric)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1676

{
  "value": [
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
  ]
}
```

