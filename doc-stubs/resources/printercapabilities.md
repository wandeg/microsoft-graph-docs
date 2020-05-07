---
title: "printerCapabilities resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# printerCapabilities resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|isColorPrintingSupported|Boolean|**TODO: Add Description**|
|supportedColorConfigurations|printColorConfiguration collection|**TODO: Add Description**|
|supportedCopiesPerJob|[integerRange](../resources/integerrange.md)|**TODO: Add Description**|
|supportedDocumentMimeTypes|String collection|**TODO: Add Description**|
|supportedDuplexConfigurations|printDuplexConfiguration collection|**TODO: Add Description**|
|supportedFinishings|printFinishing collection|**TODO: Add Description**|
|supportedMediaColors|String collection|**TODO: Add Description**|
|supportedMediaSizes|String collection|**TODO: Add Description**|
|supportedMediaTypes|printMediaType collection|**TODO: Add Description**|
|supportedOrientations|printOrientation collection|**TODO: Add Description**|
|supportedOutputBins|String collection|**TODO: Add Description**|
|supportedPagesPerSheet|[integerRange](../resources/integerrange.md)|**TODO: Add Description**|
|supportedPresentationDirections|printPresentationDirection collection|**TODO: Add Description**|
|supportedPrintQualities|printQuality collection|**TODO: Add Description**|
|supportsFitPdfToPage|Boolean|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerCapabilities"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerCapabilities",
  "isColorPrintingSupported": "Boolean",
  "supportsFitPdfToPage": "Boolean",
  "supportedCopiesPerJob": {
    "@odata.type": "microsoft.graph.integerRange"
  },
  "supportedDocumentMimeTypes": [
    "String"
  ],
  "supportedFinishings": [
    "String"
  ],
  "supportedMediaColors": [
    "String"
  ],
  "supportedMediaTypes": [
    "String"
  ],
  "supportedDuplexConfigurations": [
    "String"
  ],
  "supportedMediaSizes": [
    "String"
  ],
  "supportedPagesPerSheet": {
    "@odata.type": "microsoft.graph.integerRange"
  },
  "supportedOrientations": [
    "String"
  ],
  "supportedOutputBins": [
    "String"
  ],
  "supportedPresentationDirections": [
    "String"
  ],
  "supportedColorConfigurations": [
    "String"
  ],
  "supportedPrintQualities": [
    "String"
  ]
}
```

