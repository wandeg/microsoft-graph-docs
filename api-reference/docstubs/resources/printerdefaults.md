---
title: "printerDefaults resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# printerDefaults resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|copiesPerJob|Int32|**TODO: Add Description**|
|documentMimeType|String|**TODO: Add Description**|
|duplexConfiguration|printDuplexConfiguration|**TODO: Add Description**. Possible values are: `twoSidedLongEdge`, `twoSidedShortEdge`, `oneSided`.|
|finishings|printFinishing collection|**TODO: Add Description**|
|mediaColor|String|**TODO: Add Description**|
|mediaSize|String|**TODO: Add Description**|
|mediaType|printMediaType|**TODO: Add Description**. Possible values are: `stationery`, `transparency`, `envelope`, `envelopePlain`, `continuous`, `screen`, `screenPaged`, `continuousLong`, `continuousShort`, `envelopeWindow`, `multiPartForm`, `multiLayer`, `labels`.|
|orientation|printOrientation|**TODO: Add Description**. Possible values are: `portrait`, `landscape`, `reverseLandscape`, `reversePortrait`.|
|outputBin|String|**TODO: Add Description**|
|pagesPerSheet|Int32|**TODO: Add Description**|
|pdfFitToPage|Boolean|**TODO: Add Description**|
|presentationDirection|printPresentationDirection|**TODO: Add Description**. Possible values are: `clockwiseFromTopLeft`, `counterClockwiseFromTopLeft`, `counterClockwiseFromTopRight`, `clockwiseFromTopRight`, `counterClockwiseFromBottomLeft`, `clockwiseFromBottomLeft`, `counterClockwiseFromBottomRight`, `clockwiseFromBottomRight`.|
|printColorConfiguration|printColorConfiguration|**TODO: Add Description**. Possible values are: `blackAndWhite`, `grayscale`, `color`, `auto`.|
|printQuality|printQuality|**TODO: Add Description**. Possible values are: `low`, `medium`, `high`.|

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

