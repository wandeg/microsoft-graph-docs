---
title: "teleconferenceDeviceMediaQuality resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teleconferenceDeviceMediaQuality resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|averageInboundJitter|Duration||
|averageInboundPacketLossRateInPercentage|Double||
|averageInboundRoundTripDelay|Duration||
|averageOutboundJitter|Duration||
|averageOutboundPacketLossRateInPercentage|Double||
|averageOutboundRoundTripDelay|Duration||
|channelIndex|Int32||
|inboundPackets|Int64||
|localIPAddress|String||
|localPort|Int32||
|maximumInboundJitter|Duration||
|maximumInboundPacketLossRateInPercentage|Double||
|maximumInboundRoundTripDelay|Duration||
|maximumOutboundJitter|Duration||
|maximumOutboundPacketLossRateInPercentage|Double||
|maximumOutboundRoundTripDelay|Duration||
|mediaDuration|Duration||
|networkLinkSpeedInBytes|Int64||
|outboundPackets|Int64||
|remoteIPAddress|String||
|remotePort|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teleconferenceDeviceMediaQuality"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teleconferenceDeviceMediaQuality",
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
```

