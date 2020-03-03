---
title: "Get filterOperatorSchema"
description: "Read properties and relationships of the filterOperatorSchema object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get filterOperatorSchema

Read properties and relationships of the [filterOperatorSchema](../resources/filteroperatorschema.md) object.

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
GET /filterOperators/{filterOperatorsId}
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
If successful, this method returns a `200 OK` response code and [filterOperatorSchema](../resources/filteroperatorschema.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_filteroperatorschema"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/filterOperators/{filterOperatorsId}
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
    "id": "58b8aa39-aa39-58b8-39aa-b85839aab858",
    "arity": "String",
    "multivaluedComparisonType": "String",
    "supportedAttributeTypes": [
      "String"
    ]
  }
}
```

