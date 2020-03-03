---
title: "synchronizationTemplate resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# synchronizationTemplate resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get synchronizationTemplate](../api/synchronizationtemplate-get.md)|[synchronizationTemplate](../resources/synchronizationTemplate.md)|Read properties and relationships of the [synchronizationTemplate](../resources/synchronizationtemplate.md) object.|
|[Delete synchronizationTemplate](../api/synchronizationtemplate-delete.md)|None|Deletes a [synchronizationTemplate](../resources/synchronizationtemplate.md).|
|[Update synchronizationTemplate](../api/synchronizationtemplate-update.md)|[synchronizationTemplate](../resources/synchronizationTemplate.md)|Update the properties of a [synchronizationTemplate](../resources/synchronizationtemplate.md) object.|
|[Get synchronizationSchema](../api/synchronizationschema-get.md)|[synchronizationSchema](../resources/synchronizationSchema.md)|Read properties and relationships of the [synchronizationSchema](../resources/synchronizationschema.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationId|Guid||
|default|Boolean||
|description|String||
|discoverable|Boolean||
|factoryTag|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|metadata|[metadataEntry](../resources/metadataEntry.md) collection||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|schema|[synchronizationSchema](../resources/synchronizationSchema.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationTemplate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationTemplate",
  "id": "String (identifier)",
  "applicationId": "Guid",
  "default": true,
  "description": "String",
  "discoverable": true,
  "factoryTag": "String",
  "metadata": [
    {
      "@odata.type": "microsoft.graph.metadataEntry"
    }
  ]
}
```

