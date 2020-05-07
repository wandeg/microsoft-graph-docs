---
title: "dimension resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# dimension resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List dimensionValues](../api/dimension-list-dimensionvalues.md)|[dimensionValue](../resources/dimensionvalue.md) collection|Get the dimensionValues from the dimensionValues navigation property.|
|[Create dimensionValues](../api/dimension-post-dimensionvalues.md)|[dimensionValue](../resources/dimensionvalue.md)|Create a new dimensionValues object.|
|[Delete dimensionValues](../api/dimension-delete-dimensionvalues.md)|None|Delete a [dimensionValue](../resources/dimensionvalue.md) object.|
|[Update dimensionValues](../api/dimension-update-dimensionvalues.md)|[dimensionValue](../resources/dimensionvalue.md)|Update the properties of a dimensionValues object.|
|[Get dimensionValue](../api/dimensionvalue-get.md)|[dimensionValue](../resources/dimensionvalue.md)|Read the properties and relationships of a [dimensionValue](../resources/dimensionvalue.md) object.|
|[List dimensions](../api/company-list-dimensions.md)|[dimension](../resources/dimension.md) collection|Get the dimensions from the dimensions navigation property.|
|[Create dimensions](../api/company-post-dimensions.md)|[dimension](../resources/dimension.md)|Create a new dimensions object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|dimensionValues|[dimensionValue](../resources/dimensionvalue.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dimension",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dimension",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

