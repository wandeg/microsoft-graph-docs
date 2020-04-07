---
title: "teleconferenceDeviceQuality resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teleconferenceDeviceQuality resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|callChainId|Guid||
|cloudServiceDeploymentEnvironment|String||
|cloudServiceDeploymentId|String||
|cloudServiceInstanceName|String||
|cloudServiceName|String||
|deviceDescription|String||
|deviceName|String||
|mediaLegId|Guid||
|mediaQualityList|[teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md) collection||
|participantId|Guid||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teleconferenceDeviceQuality"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teleconferenceDeviceQuality",
  "callChainId": "Guid",
  "participantId": "Guid",
  "mediaLegId": "Guid",
  "deviceName": "String",
  "deviceDescription": "String",
  "cloudServiceName": "String",
  "cloudServiceInstanceName": "String",
  "cloudServiceDeploymentId": "String",
  "cloudServiceDeploymentEnvironment": "String",
  "mediaQualityList": [
    {
      "@odata.type": "microsoft.graph.teleconferenceDeviceAudioQuality",
      "channelIndex": 1024,
      "mediaDuration": "String (duration)",
      "networkLinkSpeedInBytes": 1024,
      "localIPAddress": "String",
      "localPort": 1024,
      "remoteIPAddress": "String",
      "remotePort": 1024,
      "inboundPackets": 1024,
      "outboundPackets": 1024,
      "averageInboundPacketLossRateInPercentage": "Double",
      "averageOutboundPacketLossRateInPercentage": "Double",
      "maximumInboundPacketLossRateInPercentage": "Double",
      "maximumOutboundPacketLossRateInPercentage": "Double",
      "averageInboundRoundTripDelay": "String (duration)",
      "averageOutboundRoundTripDelay": "String (duration)",
      "maximumInboundRoundTripDelay": "String (duration)",
      "maximumOutboundRoundTripDelay": "String (duration)",
      "averageInboundJitter": "String (duration)",
      "averageOutboundJitter": "String (duration)",
      "maximumInboundJitter": "String (duration)",
      "maximumOutboundJitter": "String (duration)"
    }
  ]
}
```

