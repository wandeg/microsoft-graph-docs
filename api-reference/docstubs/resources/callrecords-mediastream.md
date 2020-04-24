---
title: "mediaStream resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mediaStream resource type


Namespace: microsoft.graph.callRecords

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|averageAudioDegradation|Single|**TODO: Add Description**|
|averageAudioNetworkJitter|Duration|**TODO: Add Description**|
|averageBandwidthEstimate|Int64|**TODO: Add Description**|
|averageJitter|Duration|**TODO: Add Description**|
|averagePacketLossRate|Single|**TODO: Add Description**|
|averageRatioOfConcealedSamples|Single|**TODO: Add Description**|
|averageReceivedFrameRate|Single|**TODO: Add Description**|
|averageRoundTripTime|Duration|**TODO: Add Description**|
|averageVideoFrameLossPercentage|Single|**TODO: Add Description**|
|averageVideoFrameRate|Single|**TODO: Add Description**|
|averageVideoPacketLossRate|Single|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|lowFrameRateRatio|Single|**TODO: Add Description**|
|lowVideoProcessingCapabilityRatio|Single|**TODO: Add Description**|
|maxAudioNetworkJitter|Duration|**TODO: Add Description**|
|maxJitter|Duration|**TODO: Add Description**|
|maxPacketLossRate|Single|**TODO: Add Description**|
|maxRatioOfConcealedSamples|Single|**TODO: Add Description**|
|maxRoundTripTime|Duration|**TODO: Add Description**|
|packetUtilization|Int64|**TODO: Add Description**|
|postForwardErrorCorrectionPacketLossRate|Single|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|streamDirection|mediaStreamDirection|**TODO: Add Description**. Possible values are: `callerToCallee`, `calleeToCaller`.|
|streamId|String|**TODO: Add Description**|
|wasMediaBypassed|Boolean|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

