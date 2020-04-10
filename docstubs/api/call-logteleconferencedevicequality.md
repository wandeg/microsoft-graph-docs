---
title: "call: logTeleconferenceDeviceQuality"
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
    "callChainId": "bf4416f3-16f3-bf44-f316-44bff31644bf",
    "participantId": "349c6326-6326-349c-2663-9c3426639c34",
    "mediaLegId": "a47076f3-76f3-a470-f376-70a4f37670a4",
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
        "mediaDuration": "PT1M40.0377667S",
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
        "averageInboundRoundTripDelay": "-PT3M16.8594241S",
        "averageOutboundRoundTripDelay": "PT3M17.4665722S",
        "maximumInboundRoundTripDelay": "PT1M17.3258163S",
        "maximumOutboundRoundTripDelay": "PT11.5000551S",
        "averageInboundJitter": "PT1M9.7500958S",
        "averageOutboundJitter": "-PT31.1325666S",
        "maximumInboundJitter": "-PT1M45.2345819S",
        "maximumOutboundJitter": "-PT1M42.8728715S"
      }
    ]
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

