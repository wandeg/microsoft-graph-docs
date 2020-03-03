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
|[List fileClassificationRequests](../api/fileclassificationrequest-list.md)|[fileClassificationRequest](../resources/fileclassificationrequest.md) collection|List properties and relationships of the [fileClassificationRequest](../resources/fileclassificationrequest.md) objects.|
|[Get fileClassificationRequest](../api/fileclassificationrequest-get.md)|[fileClassificationRequest](../resources/fileclassificationrequest.md)|Read properties and relationships of the [fileClassificationRequest](../resources/fileclassificationrequest.md) object.|
|[Create fileClassificationRequest](../api/fileclassificationrequest-create.md)|[fileClassificationRequest](../resources/fileclassificationrequest.md)|Create a new [fileClassificationRequest](../resources/fileclassificationrequest.md) object.|
|[Delete fileClassificationRequest](../api/fileclassificationrequest-delete.md)|None|Deletes a [fileClassificationRequest](../resources/fileclassificationrequest.md).|
|[Update fileClassificationRequest](../api/fileclassificationrequest-update.md)|[fileClassificationRequest](../resources/fileclassificationrequest.md)|Update the properties of a [fileClassificationRequest](../resources/fileclassificationrequest.md) object.|
|[List classifyFile](../api/dataclassificationservice-list-classifyfile.md)|[fileClassificationRequest](../resources/fileclassificationrequest.md) collection|Get the fileClassificationRequests from the classifyFile navigation property.|
|[Add classifyFile](../api/dataclassificationservice-post-classifyfile.md)|[fileClassificationRequest](../resources/fileclassificationrequest.md)|Add classifyFile by posting to the classifyFile collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|file|Stream||
|id|String| Inherited from [entity](../resources/entity.md)|
|sensitiveTypeIds|String collection||

## Relationships
None

## JSON Representation
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

