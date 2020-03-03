---
title: "media resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# media resource type


Namespace: microsoft.graph.callRecords



## Properties
|Property|Type|Description|
|:---|:---|:---|
|calleeDevice|[deviceInfo](../resources/callrecords-deviceinfo.md)||
|calleeNetwork|[networkInfo](../resources/callrecords-networkinfo.md)||
|callerDevice|[deviceInfo](../resources/callrecords-deviceinfo.md)||
|callerNetwork|[networkInfo](../resources/callrecords-networkinfo.md)||
|label|String||
|streams|[mediaStream](../resources/callrecords-mediastream.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.media"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.media",
  "label": "String",
  "callerNetwork": {
    "@odata.type": "microsoft.graph.callRecords.networkInfo",
    "ipAddress": "String",
    "subnet": "String",
    "linkSpeed": 1024,
    "connectionType": "String",
    "port": 1024,
    "reflexiveIPAddress": "String",
    "relayIPAddress": "String",
    "relayPort": 1024,
    "macAddress": "String",
    "wifiMicrosoftDriver": "String",
    "wifiMicrosoftDriverVersion": "String",
    "wifiVendorDriver": "String",
    "wifiVendorDriverVersion": "String",
    "wifiChannel": 1024,
    "wifiBand": "String",
    "basicServiceSetIdentifier": "String",
    "wifiRadioType": "String",
    "wifiSignalStrength": 1024,
    "wifiBatteryCharge": 1024,
    "dnsSuffix": "String",
    "sentQualityEventRatio": "Single",
    "receivedQualityEventRatio": "Single",
    "delayEventRatio": "Single",
    "bandwidthLowEventRatio": "Single"
  },
  "calleeNetwork": {
    "@odata.type": "microsoft.graph.callRecords.networkInfo"
  },
  "callerDevice": {
    "@odata.type": "microsoft.graph.callRecords.deviceInfo",
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
  },
  "calleeDevice": {
    "@odata.type": "microsoft.graph.callRecords.deviceInfo"
  },
  "streams": [
    {
      "@odata.type": "microsoft.graph.callRecords.mediaStream",
      "streamId": "String",
      "startDateTime": "String (timestamp)",
      "endDateTime": "String (timestamp)",
      "streamDirection": "String",
      "averageAudioDegradation": "Single",
      "averageJitter": "String (duration)",
      "maxJitter": "String (duration)",
      "averagePacketLossRate": "Single",
      "maxPacketLossRate": "Single",
      "averageRatioOfConcealedSamples": "Single",
      "maxRatioOfConcealedSamples": "Single",
      "averageRoundTripTime": "String (duration)",
      "maxRoundTripTime": "String (duration)",
      "packetUtilization": 1024,
      "averageBandwidthEstimate": 1024,
      "wasMediaBypassed": true,
      "postForwardErrorCorrectionPacketLossRate": "Single",
      "averageVideoFrameLossPercentage": "Single",
      "averageReceivedFrameRate": "Single",
      "lowFrameRateRatio": "Single",
      "averageVideoPacketLossRate": "Single",
      "averageVideoFrameRate": "Single",
      "lowVideoProcessingCapabilityRatio": "Single",
      "averageAudioNetworkJitter": "String (duration)",
      "maxAudioNetworkJitter": "String (duration)"
    }
  ]
}
```

