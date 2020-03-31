---
title: "printerCapabilities resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# printerCapabilities resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|isColorPrintingSupported|Boolean||
|supportedColorConfigurations|Enumeration collection||
|supportedCopiesPerJob|[integerRange](../resources/integerrange.md)||
|supportedDocumentMimeTypes|String collection||
|supportedDuplexConfigurations|Enumeration collection||
|supportedFinishings|Enumeration collection||
|supportedMediaColors|String collection||
|supportedMediaSizes|String collection||
|supportedMediaTypes|Enumeration collection||
|supportedOrientations|Enumeration collection||
|supportedOutputBins|String collection||
|supportedPagesPerSheet|[integerRange](../resources/integerrange.md)||
|supportedPresentationDirections|Enumeration collection||
|supportedPrintQualities|Enumeration collection||
|supportsFitPdfToPage|Boolean||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerCapabilities"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerCapabilities",
  "isColorPrintingSupported": true,
  "supportsFitPdfToPage": true,
  "supportedCopiesPerJob": {
    "@odata.type": "microsoft.graph.integerRange",
    "minimum": 1024,
    "maximum": 1024
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

