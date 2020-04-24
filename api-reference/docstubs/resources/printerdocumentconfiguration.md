---
title: "printerDocumentConfiguration resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# printerDocumentConfiguration resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|colorConfiguration|printColorConfiguration|**TODO: Add Description**. Possible values are: `blackAndWhite`, `grayscale`, `color`, `auto`.|
|copies|Int32|**TODO: Add Description**|
|duplexConfiguration|printDuplexConfiguration|**TODO: Add Description**. Possible values are: `twoSidedLongEdge`, `twoSidedShortEdge`, `oneSided`.|
|feedDirection|printerFeedDirection|**TODO: Add Description**. Possible values are: `longEdgeFirst`, `shortEdgeFirst`.|
|orientation|printOrientation|**TODO: Add Description**. Possible values are: `portrait`, `landscape`, `reverseLandscape`, `reversePortrait`.|
|pageRanges|[printPageRange](../resources/printpagerange.md) collection|**TODO: Add Description**|
|printQuality|printQuality|**TODO: Add Description**. Possible values are: `low`, `medium`, `high`.|
|printResolutionInDpi|Int32|**TODO: Add Description**|

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

