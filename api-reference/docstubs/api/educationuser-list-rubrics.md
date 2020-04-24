---
title: "List rubrics"
description: "Get the educationRubrics from the rubrics navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List rubrics

Namespace: microsoft.graph

Get the educationRubrics from the rubrics navigation property.

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
GET /education/classes/{educationClassId}/members/{educationUserId}/rubrics
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [educationRubric](../resources/educationrubric.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_educationrubric"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{educationClassId}/members/{educationUserId}/rubrics
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationrubric)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

