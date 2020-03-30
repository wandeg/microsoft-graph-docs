---
title: "List rubrics"
description: "Get the educationRubrics from the rubrics navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List rubrics

Namespace: microsoft.graph

Get the educationRubrics from the rubrics navigation property.

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
GET /education/classes/{educationClassId}/members/{educationUserId}/rubrics
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
If successful, this method returns a `200 OK` response code and a collection of [educationRubric](../resources/educationrubric.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationrubric"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{educationClassId}/members/{educationUserId}/rubrics
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
Content-Length: 1677

{
  "value": [
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
  ]
}
```

