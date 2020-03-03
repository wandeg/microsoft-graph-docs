---
title: "textClassificationRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# textClassificationRequest resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get textClassificationRequest](../api/textclassificationrequest-get.md)|[textClassificationRequest](../resources/textClassificationRequest.md)|Read properties and relationships of the [textClassificationRequest](../resources/textclassificationrequest.md) object.|
|[Delete textClassificationRequest](../api/textclassificationrequest-delete.md)|None|Deletes a [textClassificationRequest](../resources/textclassificationrequest.md).|
|[Update textClassificationRequest](../api/textclassificationrequest-update.md)|[textClassificationRequest](../resources/textClassificationRequest.md)|Update the properties of a [textClassificationRequest](../resources/textclassificationrequest.md) object.|
|[List classifyText](../api/dataclassificationservice-list-classifytext.md)|[textClassificationRequest](../resources/textClassificationRequest.md) collection|Get the textClassificationRequests from the classifyText navigation property.|
|[Add classifyText](../api/dataclassificationservice-post-classifytext.md)|[textClassificationRequest](../resources/textClassificationRequest.md)|Add classifyText by posting to the classifyText collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|scopesToRun|Enumeration|. Possible values are: `fullDocument`, `partialDocument`.|
|sensitiveTypeIds|String collection||
|text|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.textClassificationRequest",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.textClassificationRequest",
  "id": "String (identifier)",
  "text": "String",
  "sensitiveTypeIds": [
    "String"
  ],
  "scopesToRun": "String"
}
```

