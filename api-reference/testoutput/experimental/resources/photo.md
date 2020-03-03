---
title: "photo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# photo resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|cameraMake|String||
|cameraModel|String||
|exposureDenominator|Double||
|exposureNumerator|Double||
|fNumber|Double||
|focalLength|Double||
|iso|Int32||
|orientation|Int16||
|takenDateTime|DateTimeOffset||

## Relationships
None

## JSON Representation
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

