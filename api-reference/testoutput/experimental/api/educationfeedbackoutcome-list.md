---
title: "List educationFeedbackOutcomes"
description: "List properties and relationships of the educationFeedbackOutcome objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List educationFeedbackOutcomes

Namespace: microsoft.graph

List properties and relationships of the [educationFeedbackOutcome](../resources/educationfeedbackoutcome.md) objects.

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
GET ** Collection URI for microsoft.graph.educationFeedbackOutcome not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [educationFeedbackOutcome](../resources/educationfeedbackoutcome.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_educationfeedbackoutcome"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.educationFeedbackOutcome not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.educationfeedbackoutcome)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1171

{
  "value": [
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
  ]
}
```

