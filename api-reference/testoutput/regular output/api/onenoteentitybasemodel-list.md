---
title: "List onenoteEntityBaseModels"
description: "List properties and relationships of the onenoteEntityBaseModel objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List onenoteEntityBaseModels

Namespace: microsoft.graph

List properties and relationships of the [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md) objects.

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
GET ** Collection URI for microsoft.graph.onenoteEntityBaseModel not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onenoteentitybasemodel"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.onenoteEntityBaseModel not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.onenoteentitybasemodel)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 183

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.onenoteEntityBaseModel",
      "id": "3ab54c4d-4c4d-3ab5-4d4c-b53a4d4cb53a",
      "self": "Self value"
    }
  ]
}
```

