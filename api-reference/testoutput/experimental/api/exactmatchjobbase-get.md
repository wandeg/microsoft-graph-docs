---
title: "Get exactMatchJobBase"
description: "Read properties and relationships of the exactMatchJobBase object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get exactMatchJobBase

Read properties and relationships of the [exactMatchJobBase](../resources/exactmatchjobbase.md) object.

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
GET ** Entity URI for microsoft.graph.exactMatchJobBase not found
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
If successful, this method returns a `200 OK` response code and [exactMatchJobBase](../resources/exactmatchjobbase.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_exactmatchjobbase"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.exactMatchJobBase not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.exactMatchJobBase"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 941

{
  "value": {
    "@odata.type": "#microsoft.graph.exactMatchJobBase",
    "id": "8db4424b-424b-8db4-4b42-b48d4b42b48d",
    "creationDateTime": "2017-01-01T00:00:59.0982804+03:00",
    "startDateTime": "2017-01-01T00:03:15.6077862+03:00",
    "lastUpdatedDateTime": "2017-01-01T00:01:04.1563754+03:00",
    "completionDateTime": "2017-01-01T00:02:23.013137+03:00",
    "error": {
      "@odata.type": "microsoft.graph.classificationError",
      "code": "Code value",
      "message": "Message value",
      "target": "Target value",
      "innerError": {
        "@odata.type": "microsoft.graph.classificationInnerError",
        "errorDateTime": "2017-01-01T00:03:21.298689+03:00",
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
}
```

