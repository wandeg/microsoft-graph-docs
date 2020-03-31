---
title: "logTeleconferenceDeviceQuality"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# logTeleconferenceDeviceQuality

Namespace: microsoft.graph



## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /app/calls/logTeleconferenceDeviceQuality
POST /communications/calls/logTeleconferenceDeviceQuality
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|quality|[teleconferenceDeviceQuality](../resources/teleconferencedevicequality.md)||



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "call_logteleconferencedevicequality"
}
-->
``` http
POST https://graph.microsoft.com/beta/app/calls/logTeleconferenceDeviceQuality

Content-type: application/json
Content-length: 1814

{
  "quality": {
    "@odata.type": "microsoft.graph.teleconferenceDeviceQuality",
    "callChainId": "d9d84327-4327-d9d8-2743-d8d92743d8d9",
    "participantId": "5e751e49-1e49-5e75-491e-755e491e755e",
    "mediaLegId": "3c890593-0593-3c89-9305-893c9305893c",
    "deviceName": "Device Name value",
    "deviceDescription": "Device Description value",
    "cloudServiceName": "Cloud Service Name value",
    "cloudServiceInstanceName": "Cloud Service Instance Name value",
    "cloudServiceDeploymentId": "Cloud Service Deployment Id value",
    "cloudServiceDeploymentEnvironment": "Cloud Service Deployment Environment value",
    "mediaQualityList": [
      {
        "@odata.type": "microsoft.graph.teleconferenceDeviceAudioQuality",
        "channelIndex": 12,
        "mediaDuration": "-PT11.7738441S",
        "networkLinkSpeedInBytes": 7,
        "localIPAddress": "Local IPAddress value",
        "localPort": 9,
        "remoteIPAddress": "Remote IPAddress value",
        "remotePort": 10,
        "inboundPackets": 14,
        "outboundPackets": 15,
        "averageInboundPacketLossRateInPercentage": "Double",
        "averageOutboundPacketLossRateInPercentage": "Double",
        "maximumInboundPacketLossRateInPercentage": "Double",
        "maximumOutboundPacketLossRateInPercentage": "Double",
        "averageInboundRoundTripDelay": "PT44.5928126S",
        "averageOutboundRoundTripDelay": "PT47.5293435S",
        "maximumInboundRoundTripDelay": "-PT3M20.2085231S",
        "maximumOutboundRoundTripDelay": "PT1M31.7516137S",
        "averageInboundJitter": "-PT1M21.1236068S",
        "averageOutboundJitter": "-PT1M24.9391726S",
        "maximumInboundJitter": "PT2M36.2551866S",
        "maximumOutboundJitter": "-PT3M33.1178721S"
      }
    ]
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

