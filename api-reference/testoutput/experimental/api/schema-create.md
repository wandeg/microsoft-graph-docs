---
title: "Create schema"
description: "Create a new schema object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create schema

Namespace: microsoft.graph

Create a new [schema](../resources/schema.md) object.

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
POST ** Collection URI for microsoft.graph.schema not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [schema](../resources/schema.md) object.

The following table shows the properties that are required when you create the [schema](../resources/schema.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|baseType|String||
|properties|[property](../resources/property.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [schema](../resources/schema.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_schema_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.schema not found
Content-type: application/json
Content-length: 311

{
  "@odata.type": "#microsoft.graph.schema",
  "baseType": "Base Type value",
  "properties": [
    {
      "@odata.type": "microsoft.graph.property",
      "name": "Name value",
      "type": "String",
      "isSearchable": true,
      "isRetrievable": true,
      "isQueryable": true
    }
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schema"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 360

{
  "@odata.type": "#microsoft.graph.schema",
  "id": "22a09afe-9afe-22a0-fe9a-a022fe9aa022",
  "baseType": "Base Type value",
  "properties": [
    {
      "@odata.type": "microsoft.graph.property",
      "name": "Name value",
      "type": "String",
      "isSearchable": true,
      "isRetrievable": true,
      "isQueryable": true
    }
  ]
}
```

