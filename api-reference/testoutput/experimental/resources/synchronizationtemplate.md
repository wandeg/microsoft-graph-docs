---
title: "synchronizationTemplate resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# synchronizationTemplate resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List synchronizationTemplates](../api/synchronizationtemplate-list.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md) collection|List properties and relationships of the [synchronizationTemplate](../resources/synchronizationtemplate.md) objects.|
|[Get synchronizationTemplate](../api/synchronizationtemplate-get.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md)|Read properties and relationships of the [synchronizationTemplate](../resources/synchronizationtemplate.md) object.|
|[Create synchronizationTemplate](../api/synchronizationtemplate-create.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md)|Create a new [synchronizationTemplate](../resources/synchronizationtemplate.md) object.|
|[Delete synchronizationTemplate](../api/synchronizationtemplate-delete.md)|None|Deletes a [synchronizationTemplate](../resources/synchronizationtemplate.md).|
|[Update synchronizationTemplate](../api/synchronizationtemplate-update.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md)|Update the properties of a [synchronizationTemplate](../resources/synchronizationtemplate.md) object.|
|[Get synchronizationSchema](../api/synchronizationschema-get.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Read properties and relationships of the [synchronizationSchema](../resources/synchronizationschema.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationId|Guid||
|default|Boolean||
|description|String||
|discoverable|Boolean||
|factoryTag|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|metadata|[metadataEntry](../resources/metadataentry.md) collection||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|schema|[synchronizationSchema](../resources/synchronizationschema.md)||

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

