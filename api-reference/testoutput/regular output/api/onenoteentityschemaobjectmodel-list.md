---
title: "List onenoteEntitySchemaObjectModels"
description: "List properties and relationships of the onenoteEntitySchemaObjectModel objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List onenoteEntitySchemaObjectModels

Namespace: microsoft.graph

List properties and relationships of the [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md) objects.

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
GET ** Collection URI for microsoft.graph.onenoteEntitySchemaObjectModel not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onenoteentityschemaobjectmodel"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.onenoteEntitySchemaObjectModel not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.onenoteentityschemaobjectmodel)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 253

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.onenoteEntitySchemaObjectModel",
      "id": "765559c3-59c3-7655-c359-5576c3595576",
      "self": "Self value",
      "createdDateTime": "2017-01-01T00:02:24.618735+03:00"
    }
  ]
}
```

