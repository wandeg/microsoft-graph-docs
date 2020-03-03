---
title: "Update educationFeedbackOutcome"
description: "Update the properties of a educationFeedbackOutcome object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update educationFeedbackOutcome

Namespace: microsoft.graph

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
In the request body, supply a JSON representation for the [educationFeedbackOutcome](../resources/educationfeedbackoutcome.md) object.

The following table shows the properties that are required when you create the [educationFeedbackOutcome](../resources/educationfeedbackoutcome.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [educationOutcome](../resources/educationoutcome.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [educationOutcome](../resources/educationoutcome.md)|
|feedback|[educationFeedback](../resources/educationfeedback.md)||
|publishedFeedback|[educationFeedback](../resources/educationfeedback.md)||



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
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.educationFeedbackOutcome not found
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
    "feedbackDateTime": "2016-12-31T23:59:51.6026372+03:00",
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
  "id": "70150078-0078-7015-7800-157078001570",
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
  "feedback": {
    "@odata.type": "microsoft.graph.educationFeedback",
    "text": {
      "@odata.type": "microsoft.graph.educationItemBody",
      "contentType": "String",
      "content": "Content value"
    },
    "feedbackDateTime": "2016-12-31T23:59:51.6026372+03:00",
    "feedbackBy": {
      "@odata.type": "microsoft.graph.identitySet"
    }
  },
  "publishedFeedback": {
    "@odata.type": "microsoft.graph.educationFeedback"
  }
}
```

