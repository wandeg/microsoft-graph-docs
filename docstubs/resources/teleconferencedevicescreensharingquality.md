---
title: "teleconferenceDeviceScreenSharingQuality resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# teleconferenceDeviceScreenSharingQuality resource type


Namespace: microsoft.graph




Inherits from [teleconferenceDeviceVideoQuality](../resources/teleconferencedevicevideoquality.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|averageInboundBitRate|Double| Inherited from [teleconferenceDeviceVideoQuality](../resources/teleconferencedevicevideoquality.md)|
|averageInboundFrameRate|Double| Inherited from [teleconferenceDeviceVideoQuality](../resources/teleconferencedevicevideoquality.md)|
|averageInboundJitter|Duration| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|averageInboundPacketLossRateInPercentage|Double| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|averageInboundRoundTripDelay|Duration| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|averageOutboundBitRate|Double| Inherited from [teleconferenceDeviceVideoQuality](../resources/teleconferencedevicevideoquality.md)|
|averageOutboundFrameRate|Double| Inherited from [teleconferenceDeviceVideoQuality](../resources/teleconferencedevicevideoquality.md)|
|averageOutboundJitter|Duration| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|averageOutboundPacketLossRateInPercentage|Double| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|averageOutboundRoundTripDelay|Duration| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|channelIndex|Int32| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|inboundPackets|Int64| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|localIPAddress|String| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|localPort|Int32| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|maximumInboundJitter|Duration| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|maximumInboundPacketLossRateInPercentage|Double| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|maximumInboundRoundTripDelay|Duration| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|maximumOutboundJitter|Duration| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|maximumOutboundPacketLossRateInPercentage|Double| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|maximumOutboundRoundTripDelay|Duration| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|mediaDuration|Duration| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|networkLinkSpeedInBytes|Int64| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|outboundPackets|Int64| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|remoteIPAddress|String| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|
|remotePort|Int32| Inherited from [teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teleconferenceDeviceScreenSharingQuality"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teleconferenceDeviceScreenSharingQuality",
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
  "maximumOutboundJitter": "String (duration)",
  "averageInboundFrameRate": "Double",
  "averageOutboundFrameRate": "Double",
  "averageInboundBitRate": "Double",
  "averageOutboundBitRate": "Double"
}
```

