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
|[Get synchronizationTemplate](../api/synchronizationtemplate-get.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md)|Read properties and relationships of the [synchronizationTemplate](../resources/synchronizationtemplate.md) object.|
|[Update synchronizationTemplate](../api/synchronizationtemplate-update.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md)|Update the properties of a [synchronizationTemplate](../resources/synchronizationtemplate.md) object.|
|[Get synchronizationSchema](../api/synchronizationschema-get.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Read properties and relationships of the [synchronizationSchema](../resources/synchronizationschema.md) object.|
|[List templates](../api/synchronization-list-templates.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md) collection|Get the synchronizationTemplates from the templates navigation property.|
|[Add templates](../api/synchronization-post-templates.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md)|Add templates by posting to the templates collection.|

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

## JSON representation
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

