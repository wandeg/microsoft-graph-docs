---
title: "Update schemaExtension"
description: "Update the properties of a schemaExtension object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update schemaExtension

Namespace: microsoft.graph

Update the properties of a [schemaExtension](../resources/schemaextension.md) object.

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
PATCH /schemaExtensions/{schemaExtensionsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [schemaExtension](../resources/schemaextension.md) object.

The following table shows the properties that are required when you create the [schemaExtension](../resources/schemaextension.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|description|String|**TODO: Add Description**|
|targetTypes|String collection|**TODO: Add Description**|
|properties|[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|owner|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [schemaExtension](../resources/schemaextension.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_schemaextension"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/schemaExtensions/{schemaExtensionsId}
Content-Type: application/json
Content-length: 365

{
  "@odata.type": "#microsoft.graph.schemaExtension",
  "description": "Description value",
  "targetTypes": [
    "Target Types value"
  ],
  "properties": [
    {
      "@odata.type": "microsoft.graph.extensionSchemaProperty",
      "name": "Name value",
      "type": "Type value"
    }
  ],
  "status": "Status value",
  "owner": "Owner value"
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
  "@odata.type": "#microsoft.graph.schemaExtension",
  "id": "7a4131b7-31b7-7a41-b731-417ab731417a",
  "description": "Description value",
  "targetTypes": [
    "Target Types value"
  ],
  "properties": [
    {
      "@odata.type": "microsoft.graph.extensionSchemaProperty",
      "name": "Name value",
      "type": "Type value"
    }
  ],
  "status": "Status value",
  "owner": "Owner value"
}
```

