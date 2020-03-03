---
title: "Update attributeMappingFunctionSchema"
description: "Update the properties of a attributeMappingFunctionSchema object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update attributeMappingFunctionSchema

Update the properties of a [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) object.

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
PATCH /functions/{functionsId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [attributeMappingFunctionSchema](../resources/attributeMappingFunctionSchema.md) object.

The following table shows the properties that are required when you create the [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|parameters|[attributeMappingParameterSchema](../resources/attributeMappingParameterSchema.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_attributemappingfunctionschema"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/functions/{functionsId}
Content-type: application/json
Content-length: 303

{
  "@odata.type": "#microsoft.graph.attributeMappingFunctionSchema",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 352

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
```

