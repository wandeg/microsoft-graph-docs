---
title: "Create androidManagedStoreAppConfigurationSchemas"
description: "Create a new androidManagedStoreAppConfigurationSchemas object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create androidManagedStoreAppConfigurationSchemas

Namespace: microsoft.graph

Create a new androidManagedStoreAppConfigurationSchemas object.

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
POST /deviceManagement/androidManagedStoreAppConfigurationSchemas
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md) object.

The following table shows the properties that are required when you create the [androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|exampleJson|Binary|**TODO: Add Description**|
|schemaItems|[androidManagedStoreAppConfigurationSchemaItem](../resources/androidmanagedstoreappconfigurationschemaitem.md) collection|**TODO: Add Description**|
|nestedSchemaItems|[androidManagedStoreAppConfigurationSchemaItem](../resources/androidmanagedstoreappconfigurationschemaitem.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_androidmanagedstoreappconfigurationschema_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAppConfigurationSchemas
Content-Type: application/json
Content-length: 369

{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "exampleJson": "Binary",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
    }
  ],
  "nestedSchemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
    }
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.androidmanagedstoreappconfigurationschema"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "id": "63efc338-c338-63ef-38c3-ef6338c3ef63",
  "exampleJson": "Binary",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
    }
  ],
  "nestedSchemaItems": [
    {
      "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchemaItem"
    }
  ]
}
```

