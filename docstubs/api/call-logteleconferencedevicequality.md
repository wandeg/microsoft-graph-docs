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
Content-length: 1808

{
  "quality": {
    "@odata.type": "microsoft.graph.teleconferenceDeviceQuality",
    "callChainId": "76f2240d-240d-76f2-0d24-f2760d24f276",
    "participantId": "e59eb673-b673-e59e-73b6-9ee573b69ee5",
    "mediaLegId": "3674427d-427d-3674-7d42-74367d427436",
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
        "mediaDuration": "-PT2M21.9196476S",
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
        "averageInboundRoundTripDelay": "PT1M3.5627853S",
        "averageOutboundRoundTripDelay": "-PT4.5367209S",
        "maximumInboundRoundTripDelay": "PT21.57697S",
        "maximumOutboundRoundTripDelay": "PT41.5405533S",
        "averageInboundJitter": "PT2M40.3144706S",
        "averageOutboundJitter": "PT3M12.888152S",
        "maximumInboundJitter": "-PT2M33.6518962S",
        "maximumOutboundJitter": "-PT3M15.7941283S"
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

