---
title: "inferenceClassification resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# inferenceClassification resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List inferenceClassifications](../api/inferenceclassification-list.md)|[inferenceClassification](../resources/inferenceClassification.md) collection|List properties and relationships of the [inferenceClassification](../resources/inferenceclassification.md) objects.|
|[Get inferenceClassification](../api/inferenceclassification-get.md)|[inferenceClassification](../resources/inferenceClassification.md)|Read properties and relationships of the [inferenceClassification](../resources/inferenceclassification.md) object.|
|[Create inferenceClassification](../api/inferenceclassification-create.md)|[inferenceClassification](../resources/inferenceClassification.md)|Create a new [inferenceClassification](../resources/inferenceclassification.md) object.|
|[Delete inferenceClassification](../api/inferenceclassification-delete.md)|None|Deletes a [inferenceClassification](../resources/inferenceclassification.md).|
|[Update inferenceClassification](../api/inferenceclassification-update.md)|[inferenceClassification](../resources/inferenceClassification.md)|Update the properties of a [inferenceClassification](../resources/inferenceclassification.md) object.|
|[List overrides](../api/inferenceclassification-list-overrides.md)|[inferenceClassificationOverride](../resources/inferenceClassificationOverride.md) collection|Get the inferenceClassificationOverrides from the overrides navigation property.|
|[Add overrides](../api/inferenceclassification-post-overrides.md)|[inferenceClassificationOverride](../resources/inferenceClassificationOverride.md)|Add overrides by posting to the overrides collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|overrides|[inferenceClassificationOverride](../resources/inferenceClassificationOverride.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.inferenceClassification",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.inferenceClassification",
  "id": "String (identifier)"
}
```

