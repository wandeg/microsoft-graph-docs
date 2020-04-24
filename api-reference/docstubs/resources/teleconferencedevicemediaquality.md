---
title: "teleconferenceDeviceMediaQuality resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# teleconferenceDeviceMediaQuality resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|averageInboundJitter|Duration|**TODO: Add Description**|
|averageInboundPacketLossRateInPercentage|Double|**TODO: Add Description**|
|averageInboundRoundTripDelay|Duration|**TODO: Add Description**|
|averageOutboundJitter|Duration|**TODO: Add Description**|
|averageOutboundPacketLossRateInPercentage|Double|**TODO: Add Description**|
|averageOutboundRoundTripDelay|Duration|**TODO: Add Description**|
|channelIndex|Int32|**TODO: Add Description**|
|inboundPackets|Int64|**TODO: Add Description**|
|localIPAddress|String|**TODO: Add Description**|
|localPort|Int32|**TODO: Add Description**|
|maximumInboundJitter|Duration|**TODO: Add Description**|
|maximumInboundPacketLossRateInPercentage|Double|**TODO: Add Description**|
|maximumInboundRoundTripDelay|Duration|**TODO: Add Description**|
|maximumOutboundJitter|Duration|**TODO: Add Description**|
|maximumOutboundPacketLossRateInPercentage|Double|**TODO: Add Description**|
|maximumOutboundRoundTripDelay|Duration|**TODO: Add Description**|
|mediaDuration|Duration|**TODO: Add Description**|
|networkLinkSpeedInBytes|Int64|**TODO: Add Description**|
|outboundPackets|Int64|**TODO: Add Description**|
|remoteIPAddress|String|**TODO: Add Description**|
|remotePort|Int32|**TODO: Add Description**|

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

