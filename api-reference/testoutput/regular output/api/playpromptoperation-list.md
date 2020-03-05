---
title: "List playPromptOperations"
description: "List properties and relationships of the playPromptOperation objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List playPromptOperations

Namespace: microsoft.graph

List properties and relationships of the [playPromptOperation](../resources/playpromptoperation.md) objects.

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
GET ** Collection URI for microsoft.graph.playPromptOperation not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [playPromptOperation](../resources/playpromptoperation.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_playpromptoperation"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.playPromptOperation not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.playpromptoperation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 392

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.playPromptOperation",
      "id": "907dd68e-d68e-907d-8ed6-7d908ed67d90",
      "status": "String",
      "clientContext": "Client Context value",
      "resultInfo": {
        "@odata.type": "microsoft.graph.resultInfo",
        "code": 4,
        "subcode": 7,
        "message": "Message value"
      }
    }
  ]
}
```

