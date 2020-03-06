---
title: "androidForWorkAppConfigurationSchema resource type"
description: "Schema describing an Android for Work application's custom configurations."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidForWorkAppConfigurationSchema resource type


Namespace: microsoft.graph

Schema describing an Android for Work application's custom configurations.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get androidForWorkAppConfigurationSchema](../api/androidforworkappconfigurationschema-get.md)|[androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md)|Read properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md) object.|
|[Update androidForWorkAppConfigurationSchema](../api/androidforworkappconfigurationschema-update.md)|[androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md)|Update the properties of a [androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|exampleJson|Binary|UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app|
|id|String| Inherited from [entity](../resources/entity.md)|
|schemaItems|[androidForWorkAppConfigurationSchemaItem](../resources/androidforworkappconfigurationschemaitem.md) collection|Collection of items each representing a named configuration option in the schema|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchema",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
  "id": "String (identifier)",
  "exampleJson": "binary",
  "schemaItems": [
    {
      "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem"
    }
  ]
}
```

