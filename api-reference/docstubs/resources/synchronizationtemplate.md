---
title: "synchronizationTemplate resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# synchronizationTemplate resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get synchronizationTemplate](../api/synchronizationtemplate-get.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md)|Read the properties and relationships of a [synchronizationTemplate](../resources/synchronizationtemplate.md) object.|
|[Update synchronizationTemplate](../api/synchronizationtemplate-update.md)|[synchronizationTemplate](../resources/synchronizationtemplate.md)|Update the properties of a [synchronizationTemplate](../resources/synchronizationtemplate.md) object.|
|[List schema](../api/synchronizationtemplate-list-schema.md)|[synchronizationSchema](../resources/synchronizationschema.md) collection|Get the synchronizationSchemas from the schema navigation property.|
|[Create schema](../api/synchronizationtemplate-post-schema.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Create a new schema object.|
|[Delete schema](../api/synchronizationtemplate-delete-schema.md)|None|Delete a [synchronizationSchema](../resources/synchronizationschema.md) object.|
|[Update schema](../api/synchronizationtemplate-update-schema.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Update the properties of a schema object.|
|[Get synchronizationSchema](../api/synchronizationschema-get.md)|[synchronizationSchema](../resources/synchronizationschema.md)|Read the properties and relationships of a [synchronizationSchema](../resources/synchronizationschema.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationId|Guid|**TODO: Add Description**|
|default|Boolean|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|discoverable|Boolean|**TODO: Add Description**|
|factoryTag|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|metadata|[metadataEntry](../resources/metadataentry.md) collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|schema|[synchronizationSchema](../resources/synchronizationschema.md)|**TODO: Add Description**|

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

