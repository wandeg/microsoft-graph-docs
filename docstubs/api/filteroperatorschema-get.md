---
title: "Get filterOperatorSchema"
description: "Read properties and relationships of the filterOperatorSchema object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get filterOperatorSchema

Namespace: microsoft.graph

Read properties and relationships of the [filterOperatorSchema](../resources/filteroperatorschema.md) object.

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
GET /filterOperators/{filterOperatorsId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [filterOperatorSchema](../resources/filteroperatorschema.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_filteroperatorschema"
}
-->
``` http
GET https://graph.microsoft.com/beta/filterOperators/{filterOperatorsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.filterOperatorSchema"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "value": {
    "@odata.type": "#microsoft.graph.filterOperatorSchema",
    "id": "d94dd34d-d34d-d94d-4dd3-4dd94dd34dd9",
    "arity": "String",
    "multivaluedComparisonType": "String",
    "supportedAttributeTypes": [
      "String"
    ]
  }
}
```

