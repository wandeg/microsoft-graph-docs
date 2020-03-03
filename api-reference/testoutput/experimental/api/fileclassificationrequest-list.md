---
title: "List fileClassificationRequests"
description: "List properties and relationships of the fileClassificationRequest objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List fileClassificationRequests

Namespace: microsoft.graph

List properties and relationships of the [fileClassificationRequest](../resources/fileclassificationrequest.md) objects.

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
GET /dataClassification/classifyFile
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [fileClassificationRequest](../resources/fileclassificationrequest.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_fileclassificationrequest"
}
-->
``` http
GET https://graph.microsoft.com/localtest/dataClassification/classifyFile
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.fileclassificationrequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 257

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.fileClassificationRequest",
      "id": "25fefee6-fee6-25fe-e6fe-fe25e6fefe25",
      "file": "Stream",
      "sensitiveTypeIds": [
        "Sensitive Type Ids value"
      ]
    }
  ]
}
```

