---
title: "List commsOperations"
description: "List properties and relationships of the commsOperation objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List commsOperations

Namespace: microsoft.graph

List properties and relationships of the [commsOperation](../resources/commsoperation.md) objects.

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
GET /communications/calls/{callId}/operations
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [commsOperation](../resources/commsoperation.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_commsoperation"
}
-->
``` http
GET https://graph.microsoft.com/localtest/communications/calls/{callId}/operations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.commsoperation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 387

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsOperation",
      "id": "39ca8e0b-8e0b-39ca-0b8e-ca390b8eca39",
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

