---
title: "androidManagedStoreAppConfigurationSchema resource type"
description: "Schema describing an Android application's custom configurations."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidManagedStoreAppConfigurationSchema resource type


Namespace: microsoft.graph

Schema describing an Android application's custom configurations.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get androidManagedStoreAppConfigurationSchema](../api/androidmanagedstoreappconfigurationschema-get.md)|[androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md)|Read properties and relationships of the [androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md) object.|
|[Update androidManagedStoreAppConfigurationSchema](../api/androidmanagedstoreappconfigurationschema-update.md)|[androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md)|Update the properties of a [androidManagedStoreAppConfigurationSchema](../resources/androidmanagedstoreappconfigurationschema.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|exampleJson|Binary|UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app|
|id|String| Inherited from [entity](../resources/entity.md)|
|nestedSchemaItems|[androidManagedStoreAppConfigurationSchemaItem](../resources/androidmanagedstoreappconfigurationschemaitem.md) collection|Collection of items each representing a named configuration option in the schema. It contains a flat list of all configuration.|
|schemaItems|[androidManagedStoreAppConfigurationSchemaItem](../resources/androidmanagedstoreappconfigurationschemaitem.md) collection|Collection of items each representing a named configuration option in the schema. It only contains the root-level configuration.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppConfigurationSchema",
  "id": "String (identifier)",
  "exampleJson": "binary",
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

