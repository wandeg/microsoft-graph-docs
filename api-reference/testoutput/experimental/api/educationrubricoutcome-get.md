---
title: "Get educationRubricOutcome"
description: "Read properties and relationships of the educationRubricOutcome object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get educationRubricOutcome

Read properties and relationships of the [educationRubricOutcome](../resources/educationrubricoutcome.md) object.

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
GET ** Entity URI for microsoft.graph.educationRubricOutcome not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [educationRubricOutcome](../resources/educationrubricoutcome.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationrubricoutcome"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.educationRubricOutcome not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationRubricOutcome"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1407

{
  "value": {
    "@odata.type": "#microsoft.graph.educationRubricOutcome",
    "id": "69e6131e-131e-69e6-1e13-e6691e13e669",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "id": "Id value",
        "displayName": "Display Name value"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
    "rubricQualityFeedback": [
      {
        "@odata.type": "microsoft.graph.rubricQualityFeedbackModel",
        "qualityId": "Quality Id value",
        "feedback": {
          "@odata.type": "microsoft.graph.educationItemBody",
          "contentType": "String",
          "content": "Content value"
        }
      }
    ],
    "rubricQualitySelectedLevels": [
      {
        "@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel",
        "columnId": "Column Id value"
      }
    ],
    "publishedRubricQualityFeedback": [
      {
        "@odata.type": "microsoft.graph.rubricQualityFeedbackModel"
      }
    ],
    "publishedRubricQualitySelectedLevels": [
      {
        "@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel"
      }
    ]
  }
}
```

