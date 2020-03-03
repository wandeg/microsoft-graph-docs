---
title: "deviceInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph.callRecords
---


# deviceInfo resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|captureDeviceDriver|String||
|captureDeviceName|String||
|captureNotFunctioningEventRatio|Single||
|cpuInsufficentEventRatio|Single||
|deviceClippingEventRatio|Single||
|deviceGlitchEventRatio|Single||
|howlingEventCount|Int32||
|initialSignalLevelRootMeanSquare|Single||
|lowSpeechLevelEventRatio|Single||
|lowSpeechToNoiseEventRatio|Single||
|micGlitchRate|Single||
|receivedNoiseLevel|Int32||
|receivedSignalLevel|Int32||
|renderDeviceDriver|String||
|renderDeviceName|String||
|renderMuteEventRatio|Single||
|renderNotFunctioningEventRatio|Single||
|renderZeroVolumeEventRatio|Single||
|sentNoiseLevel|Int32||
|sentSignalLevel|Int32||
|speakerGlitchRate|Single||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.deviceInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.deviceInfo",
  "captureDeviceName": "String",
  "captureDeviceDriver": "String",
  "renderDeviceName": "String",
  "renderDeviceDriver": "String",
  "sentSignalLevel": 1024,
  "receivedSignalLevel": 1024,
  "sentNoiseLevel": 1024,
  "receivedNoiseLevel": 1024,
  "initialSignalLevelRootMeanSquare": "Single",
  "cpuInsufficentEventRatio": "Single",
  "renderNotFunctioningEventRatio": "Single",
  "captureNotFunctioningEventRatio": "Single",
  "deviceGlitchEventRatio": "Single",
  "lowSpeechToNoiseEventRatio": "Single",
  "lowSpeechLevelEventRatio": "Single",
  "deviceClippingEventRatio": "Single",
  "howlingEventCount": 1024,
  "renderZeroVolumeEventRatio": "Single",
  "renderMuteEventRatio": "Single",
  "micGlitchRate": "Single",
  "speakerGlitchRate": "Single"
}
```

