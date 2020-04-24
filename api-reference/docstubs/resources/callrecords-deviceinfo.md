---
title: "deviceInfo resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceInfo resource type


Namespace: microsoft.graph.callRecords

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|captureDeviceDriver|String|**TODO: Add Description**|
|captureDeviceName|String|**TODO: Add Description**|
|captureNotFunctioningEventRatio|Single|**TODO: Add Description**|
|cpuInsufficentEventRatio|Single|**TODO: Add Description**|
|deviceClippingEventRatio|Single|**TODO: Add Description**|
|deviceGlitchEventRatio|Single|**TODO: Add Description**|
|howlingEventCount|Int32|**TODO: Add Description**|
|initialSignalLevelRootMeanSquare|Single|**TODO: Add Description**|
|lowSpeechLevelEventRatio|Single|**TODO: Add Description**|
|lowSpeechToNoiseEventRatio|Single|**TODO: Add Description**|
|micGlitchRate|Single|**TODO: Add Description**|
|receivedNoiseLevel|Int32|**TODO: Add Description**|
|receivedSignalLevel|Int32|**TODO: Add Description**|
|renderDeviceDriver|String|**TODO: Add Description**|
|renderDeviceName|String|**TODO: Add Description**|
|renderMuteEventRatio|Single|**TODO: Add Description**|
|renderNotFunctioningEventRatio|Single|**TODO: Add Description**|
|renderZeroVolumeEventRatio|Single|**TODO: Add Description**|
|sentNoiseLevel|Int32|**TODO: Add Description**|
|sentSignalLevel|Int32|**TODO: Add Description**|
|speakerGlitchRate|Single|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

