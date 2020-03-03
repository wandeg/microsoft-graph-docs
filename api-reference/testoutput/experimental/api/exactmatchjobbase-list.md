---
title: "List exactMatchJobBases"
description: "List properties and relationships of the exactMatchJobBase objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List exactMatchJobBases

Namespace: microsoft.graph

List properties and relationships of the [exactMatchJobBase](../resources/exactmatchjobbase.md) objects.

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
GET ** Collection URI for microsoft.graph.exactMatchJobBase not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [exactMatchJobBase](../resources/exactmatchjobbase.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_exactmatchjobbase"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.exactMatchJobBase not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.exactmatchjobbase)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1003

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.exactMatchJobBase",
      "id": "1b0f8add-8add-1b0f-dd8a-0f1bdd8a0f1b",
      "creationDateTime": "2017-01-01T00:02:11.4839005+03:00",
      "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
      "lastUpdatedDateTime": "2016-12-31T23:57:46.2985547+03:00",
      "completionDateTime": "2016-12-31T23:56:58.8026209+03:00",
      "error": {
        "@odata.type": "microsoft.graph.classificationError",
        "code": "Code value",
        "message": "Message value",
        "target": "Target value",
        "innerError": {
          "@odata.type": "microsoft.graph.classificationInnerError",
          "errorDateTime": "2016-12-31T23:59:22.9712113+03:00",
          "clientRequestId": "Client Request Id value",
          "activityId": "Activity Id value"
        },
        "details": [
          {
            "@odata.type": "microsoft.graph.classifcationErrorBase"
          }
        ]
      }
    }
  ]
}
```

