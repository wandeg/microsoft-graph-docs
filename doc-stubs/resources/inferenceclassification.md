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


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List inferenceClassification](../api/user-list-inferenceclassification.md)|[inferenceClassification](../resources/inferenceclassification.md) collection|Get the inferenceClassifications from the inferenceClassification navigation property.|
|[Create inferenceClassification](../api/user-post-inferenceclassification.md)|[inferenceClassification](../resources/inferenceclassification.md)|Create a new inferenceClassification object.|
|[Delete inferenceClassification](../api/user-delete-inferenceclassification.md)|None|Delete an [inferenceClassification](../resources/inferenceclassification.md) object.|
|[Update inferenceClassification](../api/user-update-inferenceclassification.md)|[inferenceClassification](../resources/inferenceclassification.md)|Update the properties of an inferenceClassification object.|
|[Get inferenceClassification](../api/user-get-inferenceclassification.md)|[inferenceClassification](../resources/inferenceclassification.md)|Read the properties and relationships of an [inferenceClassification](../resources/inferenceclassification.md) object.|
|[List overrides](../api/inferenceclassification-list-overrides.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) collection|Get the inferenceClassificationOverrides from the overrides navigation property.|
|[Create overrides](../api/inferenceclassification-post-overrides.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)|Create a new overrides object.|
|[Delete overrides](../api/inferenceclassification-delete-overrides.md)|None|Delete an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.|
|[Update overrides](../api/inferenceclassification-update-overrides.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)|Update the properties of an overrides object.|
|[Get overrides](../api/inferenceclassification-get-inferenceclassificationoverride.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)|Read the properties and relationships of an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|overrides|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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

