---
title: "schemaExtension resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# schemaExtension resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List schemaExtensions](../api/schemaextension-list.md)|[schemaExtension](../resources/schemaextension.md) collection|Get a list of the [schemaExtension](../resources/schemaextension.md) objects and their properties.|
|[Get schemaExtension](../api/schemaextension-get.md)|[schemaExtension](../resources/schemaextension.md)|Read the properties and relationships of a [schemaExtension](../resources/schemaextension.md) object.|
|[Create schemaExtension](../api/schemaextension-post-schemaextensions.md)|[schemaExtension](../resources/schemaextension.md)|Create a new [schemaExtension](../resources/schemaextension.md) object.|
|[Delete schemaExtension](../api/schemaextension-delete.md)|None|Deletes a [schemaExtension](../resources/schemaextension.md) object.|
|[Update schemaExtension](../api/schemaextension-update.md)|[schemaExtension](../resources/schemaextension.md)|Update the properties of a [schemaExtension](../resources/schemaextension.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|owner|String|**TODO: Add Description**|
|properties|[extensionSchemaProperty](../resources/extensionschemaproperty.md) collection|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|targetTypes|String collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schemaExtension",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.schemaExtension",
  "id": "String (identifier)",
  "description": "String",
  "targetTypes": [
    "String"
  ],
  "properties": [
    {
      "@odata.type": "microsoft.graph.extensionSchemaProperty"
    }
  ],
  "status": "String",
  "owner": "String"
}
```

