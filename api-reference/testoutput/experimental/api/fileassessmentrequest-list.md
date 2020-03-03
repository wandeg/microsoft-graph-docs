---
title: "List fileAssessmentRequests"
description: "List properties and relationships of the fileAssessmentRequest objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List fileAssessmentRequests

List properties and relationships of the [fileAssessmentRequest](../resources/fileassessmentrequest.md) objects.

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
GET ** Collection URI for microsoft.graph.fileAssessmentRequest not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [fileAssessmentRequest](../resources/fileassessmentrequest.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_fileassessmentrequest"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.fileAssessmentRequest not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.fileassessmentrequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 883

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.fileAssessmentRequest",
      "id": "2badf7f2-f7f2-2bad-f2f7-ad2bf2f7ad2b",
      "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
      "contentType": "String",
      "expectedAssessment": "String",
      "category": "String",
      "status": "String",
      "requestSource": "String",
      "createdBy": {
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
      "fileName": "File Name value",
      "contentData": "Content Data value"
    }
  ]
}
```

