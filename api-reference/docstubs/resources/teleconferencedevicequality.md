---
title: "teleconferenceDeviceQuality resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# teleconferenceDeviceQuality resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|callChainId|Guid|**TODO: Add Description**|
|cloudServiceDeploymentEnvironment|String|**TODO: Add Description**|
|cloudServiceDeploymentId|String|**TODO: Add Description**|
|cloudServiceInstanceName|String|**TODO: Add Description**|
|cloudServiceName|String|**TODO: Add Description**|
|deviceDescription|String|**TODO: Add Description**|
|deviceName|String|**TODO: Add Description**|
|mediaLegId|Guid|**TODO: Add Description**|
|mediaQualityList|[teleconferenceDeviceMediaQuality](../resources/teleconferencedevicemediaquality.md) collection|**TODO: Add Description**|
|participantId|Guid|**TODO: Add Description**|

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

