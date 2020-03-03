---
title: "Get onenoteEntitySchemaObjectModel"
description: "Read properties and relationships of the onenoteEntitySchemaObjectModel object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get onenoteEntitySchemaObjectModel

Read properties and relationships of the [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md) object.

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
GET ** Entity URI for microsoft.graph.onenoteEntitySchemaObjectModel not found
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
If successful, this method returns a `200 OK` response code and [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onenoteentityschemaobjectmodel"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.onenoteEntitySchemaObjectModel not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteEntitySchemaObjectModel"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 232

{
  "value": {
    "@odata.type": "#microsoft.graph.onenoteEntitySchemaObjectModel",
    "id": "6153a3d2-a3d2-6153-d2a3-5361d2a35361",
    "self": "Self value",
    "createdDateTime": "2016-12-31T23:57:22.3554145+03:00"
  }
}
```

