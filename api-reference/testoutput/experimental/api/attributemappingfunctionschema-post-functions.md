---
title: "Create attributeMappingFunctionSchema"
description: "Create a new attributeMappingFunctionSchema object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create attributeMappingFunctionSchema

Namespace: microsoft.graph

Create a new [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) object.

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
POST /functions
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) object.

The following table shows the properties that are required when you create the [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|parameters|[attributeMappingParameterSchema](../resources/attributemappingparameterschema.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [attributeMappingFunctionSchema](../resources/attributemappingfunctionschema.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_attributemappingfunctionschema_from_functions"
}
-->
``` http
POST https://graph.microsoft.com/localtest/functions
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
  "truncated": true,
  "@odata.type": "microsoft.graph.attributemappingfunctionschema"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 352

{
  "@odata.type": "#microsoft.graph.attributeMappingFunctionSchema",
  "id": "0d1d87b6-87b6-0d1d-b687-1d0db6871d0d",
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

