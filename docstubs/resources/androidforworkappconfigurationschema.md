---
title: "androidForWorkAppConfigurationSchema resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# androidForWorkAppConfigurationSchema resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get androidForWorkAppConfigurationSchema](../api/androidforworkappconfigurationschema-get.md)|[androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md)|Read properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md) object.|
|[Update androidForWorkAppConfigurationSchema](../api/androidforworkappconfigurationschema-update.md)|[androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md)|Update the properties of a [androidForWorkAppConfigurationSchema](../resources/androidforworkappconfigurationschema.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|exampleJson|Binary||
|id|String| Inherited from [entity](../resources/entity.md)|
|schemaItems|[androidForWorkAppConfigurationSchemaItem](../resources/androidforworkappconfigurationschemaitem.md) collection||

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

