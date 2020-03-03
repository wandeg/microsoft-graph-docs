---
title: "mediaStream resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph.callRecords
---


# mediaStream resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|averageAudioDegradation|Single||
|averageAudioNetworkJitter|Duration||
|averageBandwidthEstimate|Int64||
|averageJitter|Duration||
|averagePacketLossRate|Single||
|averageRatioOfConcealedSamples|Single||
|averageReceivedFrameRate|Single||
|averageRoundTripTime|Duration||
|averageVideoFrameLossPercentage|Single||
|averageVideoFrameRate|Single||
|averageVideoPacketLossRate|Single||
|endDateTime|DateTimeOffset||
|lowFrameRateRatio|Single||
|lowVideoProcessingCapabilityRatio|Single||
|maxAudioNetworkJitter|Duration||
|maxJitter|Duration||
|maxPacketLossRate|Single||
|maxRatioOfConcealedSamples|Single||
|maxRoundTripTime|Duration||
|packetUtilization|Int64||
|postForwardErrorCorrectionPacketLossRate|Single||
|startDateTime|DateTimeOffset||
|streamDirection|Enumeration|. Possible values are: `callerToCallee`, `calleeToCaller`.|
|streamId|String||
|wasMediaBypassed|Boolean||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.mediaStream"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.mediaStream",
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
```

