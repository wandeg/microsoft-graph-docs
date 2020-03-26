---
title: "Update filterOperatorSchema"
description: "Update the properties of a filterOperatorSchema object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update filterOperatorSchema

Namespace: microsoft.graph

Update the properties of a [filterOperatorSchema](../resources/filteroperatorschema.md) object.

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
PATCH /filterOperators/{filterOperatorsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [filterOperatorSchema](../resources/filteroperatorschema.md) object.

The following table shows the properties that are required when you create the [filterOperatorSchema](../resources/filteroperatorschema.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|arity|Enumeration|. Possible values are: `Binary`, `Unary`.|
|multivaluedComparisonType|Enumeration|. Possible values are: `All`, `Any`.|
|supportedAttributeTypes|Enumeration collection|. Possible values are: `DateTime`, `Boolean`, `Binary`, `Reference`, `Integer`, `String`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [filterOperatorSchema](../resources/filteroperatorschema.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_filteroperatorschema"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/filterOperators/{filterOperatorsId}
Content-type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.filterOperatorSchema",
  "arity": "String",
  "multivaluedComparisonType": "String",
  "supportedAttributeTypes": [
    "String"
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
Content-Length: 227

{
  "@odata.type": "#microsoft.graph.filterOperatorSchema",
  "id": "50b57180-7180-50b5-8071-b5508071b550",
  "arity": "String",
  "multivaluedComparisonType": "String",
  "supportedAttributeTypes": [
    "String"
  ]
}
```

