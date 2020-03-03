---
title: "Create filterOperatorSchema"
description: "Create a new filterOperatorSchema object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create filterOperatorSchema

Namespace: microsoft.graph

Create a new [filterOperatorSchema](../resources/filteroperatorschema.md) object.

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
POST /filterOperators
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
If successful, this method returns a `201 Created` response code and a [filterOperatorSchema](../resources/filteroperatorschema.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_filteroperatorschema_from_filteroperators"
}
-->
``` http
POST https://graph.microsoft.com/localtest/filterOperators
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
  "truncated": true,
  "@odata.type": "microsoft.graph.filteroperatorschema"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 227

{
  "@odata.type": "#microsoft.graph.filterOperatorSchema",
  "id": "885b8a7a-8a7a-885b-7a8a-5b887a8a5b88",
  "arity": "String",
  "multivaluedComparisonType": "String",
  "supportedAttributeTypes": [
    "String"
  ]
}
```

