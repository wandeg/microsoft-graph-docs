---
title: "Update educationRubricOutcome"
description: "Update the properties of a educationRubricOutcome object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update educationRubricOutcome

Namespace: microsoft.graph

Update the properties of a [educationRubricOutcome](../resources/educationrubricoutcome.md) object.

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
PATCH ** Entity URI for microsoft.graph.educationRubricOutcome not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [educationRubricOutcome](../resources/educationrubricoutcome.md) object.

The following table shows the properties that are required when you create the [educationRubricOutcome](../resources/educationrubricoutcome.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [educationOutcome](../resources/educationoutcome.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [educationOutcome](../resources/educationoutcome.md)|
|rubricQualityFeedback|[rubricQualityFeedbackModel](../resources/rubricqualityfeedbackmodel.md) collection||
|rubricQualitySelectedLevels|[rubricQualitySelectedColumnModel](../resources/rubricqualityselectedcolumnmodel.md) collection||
|publishedRubricQualityFeedback|[rubricQualityFeedbackModel](../resources/rubricqualityfeedbackmodel.md) collection||
|publishedRubricQualitySelectedLevels|[rubricQualitySelectedColumnModel](../resources/rubricqualityselectedcolumnmodel.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [educationRubricOutcome](../resources/educationrubricoutcome.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_educationrubricoutcome"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.educationRubricOutcome not found
Content-type: application/json
Content-length: 814

{
  "@odata.type": "#microsoft.graph.educationRubricOutcome",
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
Content-Length: 1300

{
  "@odata.type": "#microsoft.graph.educationRubricOutcome",
  "id": "b8139c4b-9c4b-b813-4b9c-13b84b9c13b8",
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
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
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
```

