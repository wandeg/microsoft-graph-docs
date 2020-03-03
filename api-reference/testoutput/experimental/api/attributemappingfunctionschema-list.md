---
title: "List attributeMappingFunctionSchemas"
description: "List properties and relationships of the attributeMappingFunctionSchema objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List attributeMappingFunctionSchemas

List properties and relationships of the [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) objects.

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
GET /functions
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_attributemappingfunctionschema"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/functions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.attributemappingfunctionschema)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 429

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.attributeMappingFunctionSchema",
      "id": "718b8b96-8b96-718b-968b-8b71968b8b71",
      "parameters": [
        {
          "@odata.type": "microsoft.graph.attributeMappingParameterSchema",
          "allowMultipleOccurrences": true,
          "name": "Name value",
          "required": true,
          "type": "String"
        }
      ]
    }
  ]
}
```

