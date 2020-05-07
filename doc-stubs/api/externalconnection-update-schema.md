---
title: "Update schema"
description: "Update the properties of a schema object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update schema

Namespace: microsoft.graph

Update the properties of a schema object.

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
PATCH /connections/{connectionsId}/schema
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [schema](../resources/schema.md) object.

The following table shows the properties that are required when you create the [schema](../resources/schema.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|baseType|String|**TODO: Add Description**|
|properties|[property](../resources/property.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [schema](../resources/schema.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_schema"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/connections/{connectionsId}/schema
Content-Type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.schema",
  "baseType": "String",
  "properties": [
    {
      "@odata.type": "microsoft.graph.property"
    }
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
  "@odata.type": "#microsoft.graph.schema",
  "id": "019a86b6-86b6-019a-b686-9a01b6869a01",
  "baseType": "String",
  "properties": [
    {
      "@odata.type": "microsoft.graph.property"
    }
  ]
}
```

