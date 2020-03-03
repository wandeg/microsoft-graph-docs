---
title: "Update educationFeedbackOutcome"
description: "Update the properties of a educationFeedbackOutcome object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update educationFeedbackOutcome

Update the properties of a [educationFeedbackOutcome](../resources/educationfeedbackoutcome.md) object.

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
PATCH ** Entity URI for microsoft.graph.educationFeedbackOutcome not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [educationFeedbackOutcome](../resources/educationFeedbackOutcome.md) object.

The following table shows the properties that are required when you create the [educationFeedbackOutcome](../resources/educationfeedbackoutcome.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [educationOutcome](../resources/educationOutcome.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [educationOutcome](../resources/educationOutcome.md)|
|feedback|[educationFeedback](../resources/educationFeedback.md)||
|publishedFeedback|[educationFeedback](../resources/educationFeedback.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [educationFeedbackOutcome](../resources/educationfeedbackoutcome.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_educationfeedbackoutcome"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.educationFeedbackOutcome not found
Content-type: application/json
Content-length: 524

{
  "@odata.type": "#microsoft.graph.educationFeedbackOutcome",
  "feedback": {
    "@odata.type": "microsoft.graph.educationFeedback",
    "text": {
      "@odata.type": "microsoft.graph.educationItemBody",
      "contentType": "String",
      "content": "Content value"
    },
    "feedbackDateTime": "2017-01-01T00:01:35.5643881+03:00",
    "feedbackBy": {
      "@odata.type": "microsoft.graph.identitySet"
    }
  },
  "publishedFeedback": {
    "@odata.type": "microsoft.graph.educationFeedback"
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
Content-Length: 1010

{
  "@odata.type": "#microsoft.graph.educationFeedbackOutcome",
  "id": "229ad521-d521-229a-21d5-9a2221d59a22",
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
  "feedback": {
    "@odata.type": "microsoft.graph.educationFeedback",
    "text": {
      "@odata.type": "microsoft.graph.educationItemBody",
      "contentType": "String",
      "content": "Content value"
    },
    "feedbackDateTime": "2017-01-01T00:01:35.5643881+03:00",
    "feedbackBy": {
      "@odata.type": "microsoft.graph.identitySet"
    }
  },
  "publishedFeedback": {
    "@odata.type": "microsoft.graph.educationFeedback"
  }
}
```

