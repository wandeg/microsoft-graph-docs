---
title: "printerDocumentConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# printerDocumentConfiguration resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|colorConfiguration|Enumeration| Possible values are: `blackAndWhite`, `grayscale`, `color`, `auto`.|
|copies|Int32||
|duplexConfiguration|Enumeration| Possible values are: `twoSidedLongEdge`, `twoSidedShortEdge`, `oneSided`.|
|feedDirection|Enumeration| Possible values are: `longEdgeFirst`, `shortEdgeFirst`.|
|orientation|Enumeration| Possible values are: `portrait`, `landscape`, `reverseLandscape`, `reversePortrait`.|
|pageRanges|[printPageRange](../resources/printpagerange.md) collection||
|printQuality|Enumeration| Possible values are: `low`, `medium`, `high`.|
|printResolutionInDpi|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerDocumentConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerDocumentConfiguration",
  "pageRanges": [
    {
      "@odata.type": "microsoft.graph.printPageRange",
      "startPage": 1024,
      "endPage": 1024
    }
  ],
  "printQuality": "String",
  "printResolutionInDpi": 1024,
  "feedDirection": "String",
  "orientation": "String",
  "duplexConfiguration": "String",
  "copies": 1024,
  "colorConfiguration": "String"
}
```

