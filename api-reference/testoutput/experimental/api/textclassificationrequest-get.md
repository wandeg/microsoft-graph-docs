---
title: "Get textClassificationRequest"
description: "Read properties and relationships of the textClassificationRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get textClassificationRequest

Namespace: microsoft.graph

Read properties and relationships of the [textClassificationRequest](../resources/textclassificationrequest.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /dataClassification/classifyText/{textClassificationRequestId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [textClassificationRequest](../resources/textclassificationrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_textclassificationrequest"
}
-->
``` http
GET https://graph.microsoft.com/localtest/dataClassification/classifyText/{textClassificationRequestId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.textClassificationRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 265

{
  "value": {
    "@odata.type": "#microsoft.graph.textClassificationRequest",
    "id": "b28c8213-8213-b28c-1382-8cb213828cb2",
    "text": "Text value",
    "sensitiveTypeIds": [
      "Sensitive Type Ids value"
    ],
    "scopesToRun": "String"
  }
}
```

