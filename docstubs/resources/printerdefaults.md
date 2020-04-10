---
title: "printerDefaults resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# printerDefaults resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|copiesPerJob|Int32||
|documentMimeType|String||
|duplexConfiguration|Enumeration| Possible values are: `twoSidedLongEdge`, `twoSidedShortEdge`, `oneSided`.|
|finishings|Enumeration collection||
|mediaColor|String||
|mediaSize|String||
|mediaType|Enumeration| Possible values are: `stationery`, `transparency`, `envelope`, `envelopePlain`, `continuous`, `screen`, `screenPaged`, `continuousLong`, `continuousShort`, `envelopeWindow`, `multiPartForm`, `multiLayer`, `labels`.|
|orientation|Enumeration| Possible values are: `portrait`, `landscape`, `reverseLandscape`, `reversePortrait`.|
|outputBin|String||
|pagesPerSheet|Int32||
|pdfFitToPage|Boolean||
|presentationDirection|Enumeration| Possible values are: `clockwiseFromTopLeft`, `counterClockwiseFromTopLeft`, `counterClockwiseFromTopRight`, `clockwiseFromTopRight`, `counterClockwiseFromBottomLeft`, `clockwiseFromBottomLeft`, `counterClockwiseFromBottomRight`, `clockwiseFromBottomRight`.|
|printColorConfiguration|Enumeration| Possible values are: `blackAndWhite`, `grayscale`, `color`, `auto`.|
|printQuality|Enumeration| Possible values are: `low`, `medium`, `high`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerDefaults"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerDefaults",
  "copiesPerJob": 1024,
  "documentMimeType": "String",
  "finishings": [
    "String"
  ],
  "mediaColor": "String",
  "mediaType": "String",
  "mediaSize": "String",
  "pagesPerSheet": 1024,
  "orientation": "String",
  "outputBin": "String",
  "pdfFitToPage": true,
  "presentationDirection": "String",
  "printColorConfiguration": "String",
  "printQuality": "String",
  "duplexConfiguration": "String"
}
```

