---
title: "fileClassificationRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# fileClassificationRequest resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get fileClassificationRequest](../api/fileclassificationrequest-get.md)|[fileClassificationRequest](../resources/fileclassificationrequest.md)|Read properties and relationships of the [fileClassificationRequest](../resources/fileclassificationrequest.md) object.|
|[Update fileClassificationRequest](../api/fileclassificationrequest-update.md)|[fileClassificationRequest](../resources/fileclassificationrequest.md)|Update the properties of a [fileClassificationRequest](../resources/fileclassificationrequest.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|file|Stream||
|id|String| Inherited from [entity](../resources/entity.md)|
|sensitiveTypeIds|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fileClassificationRequest",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileClassificationRequest",
  "id": "String (identifier)",
  "file": "Stream",
  "sensitiveTypeIds": [
    "String"
  ]
}
```

