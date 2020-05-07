---
title: "Update filterOperatorSchema"
description: "Update the properties of a filterOperatorSchema object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update filterOperatorSchema

Namespace: microsoft.graph

Update the properties of a [filterOperatorSchema](../resources/filteroperatorschema.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

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
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [filterOperatorSchema](../resources/filteroperatorschema.md) object.

The following table shows the properties that are required when you create the [filterOperatorSchema](../resources/filteroperatorschema.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|arity|scopeOperatorType|**TODO: Add Description**. Possible values are: `Binary`, `Unary`.|
|multivaluedComparisonType|scopeOperatorMultiValuedComparisonType|**TODO: Add Description**. Possible values are: `All`, `Any`.|
|supportedAttributeTypes|attributeType collection|**TODO: Add Description**. Possible values are: `DateTime`, `Boolean`, `Binary`, `Reference`, `Integer`, `String`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [filterOperatorSchema](../resources/filteroperatorschema.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_filteroperatorschema"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/filterOperators/{filterOperatorsId}
Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.filterOperatorSchema",
  "id": "d4699d06-9d06-d469-069d-69d4069d69d4",
  "arity": "String",
  "multivaluedComparisonType": "String",
  "supportedAttributeTypes": [
    "String"
  ]
}
```

