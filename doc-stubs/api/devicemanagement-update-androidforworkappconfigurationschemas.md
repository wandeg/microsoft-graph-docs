---
title: "Update androidForWorkAppConfigurationSchemas"
description: "Update the properties of an androidForWorkAppConfigurationSchemas object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update androidForWorkAppConfigurationSchemas

Namespace: microsoft.graph

Update the properties of an androidForWorkAppConfigurationSchemas object.

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
PATCH /deviceManagement/androidForWorkAppConfigurationSchemas
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md) object.

The following table shows the properties that are required when you create the [androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|exampleJson|Binary|**TODO: Add Description**|
|schemaItems|[androidForWorkAppConfigurationSchemaItem](../resources/androidforworkappconfigurationschemaitem.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_androidforworkappconfigurationschemas"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
Content-Type: application/json
Content-length: 227

{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "exampleJson": "Binary",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem"
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
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "f27d9a7d-9a7d-f27d-7d9a-7df27d9a7df2",
  "exampleJson": "Binary",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem"
    }
  ]
}
```

