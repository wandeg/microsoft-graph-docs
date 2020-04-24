---
title: "photo resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# photo resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|cameraMake|String|**TODO: Add Description**|
|cameraModel|String|**TODO: Add Description**|
|exposureDenominator|Double|**TODO: Add Description**|
|exposureNumerator|Double|**TODO: Add Description**|
|fNumber|Double|**TODO: Add Description**|
|focalLength|Double|**TODO: Add Description**|
|iso|Int32|**TODO: Add Description**|
|orientation|Int16|**TODO: Add Description**|
|takenDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.photo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.photo",
  "cameraMake": "String",
  "cameraModel": "String",
  "exposureDenominator": "Double",
  "exposureNumerator": "Double",
  "fNumber": "Double",
  "focalLength": "Double",
  "iso": 1024,
  "orientation": 1024,
  "takenDateTime": "String (timestamp)"
}
```

