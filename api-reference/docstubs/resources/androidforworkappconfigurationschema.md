---
title: "androidForWorkAppConfigurationSchema resource type"
description: "Schema describing an Android for Work application's custom configurations."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# androidForWorkAppConfigurationSchema resource type


Namespace: microsoft.graph

Schema describing an Android for Work application's custom configurations.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get androidForWorkAppConfigurationSchema](../api/androidforworkappconfigurationschema-get.md)|[androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md)|Read the properties and relationships of an [androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md) object.|
|[Update androidForWorkAppConfigurationSchema](../api/androidforworkappconfigurationschema-update.md)|[androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md)|Update the properties of an [androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|exampleJson|Binary|UTF8 encoded byte array containing example JSON string conforming to this schema that demonstrates how to set the configuration for this app|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
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

