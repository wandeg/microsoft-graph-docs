---
title: "inferenceClassification resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# inferenceClassification resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get inferenceClassification](../api/inferenceclassification-get.md)|[inferenceClassification](../resources/inferenceclassification.md)|Read the properties and relationships of an [inferenceClassification](../resources/inferenceclassification.md) object.|
|[Update inferenceClassification](../api/inferenceclassification-update.md)|[inferenceClassification](../resources/inferenceclassification.md)|Update the properties of an [inferenceClassification](../resources/inferenceclassification.md) object.|
|[List overrides](../api/inferenceclassification-list-overrides.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) collection|Get the inferenceClassificationOverrides from the overrides navigation property.|
|[Create overrides](../api/inferenceclassification-post-overrides.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)|Create a new overrides object.|
|[Delete overrides](../api/inferenceclassification-delete-overrides.md)|None|Delete an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.|
|[Update overrides](../api/inferenceclassification-update-overrides.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)|Update the properties of an overrides object.|
|[Get inferenceClassificationOverride](../api/inferenceclassificationoverride-get.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)|Read the properties and relationships of an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|overrides|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) collection|**TODO: Add Description**|

## JSON representation
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

