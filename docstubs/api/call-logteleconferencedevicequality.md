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
Content-length: 1807

{
  "quality": {
    "@odata.type": "microsoft.graph.teleconferenceDeviceQuality",
    "callChainId": "e2444f27-4f27-e244-274f-44e2274f44e2",
    "participantId": "e36009ea-09ea-e360-ea09-60e3ea0960e3",
    "mediaLegId": "91f0779f-779f-91f0-9f77-f0919f77f091",
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
        "mediaDuration": "PT54.5670324S",
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
        "averageInboundRoundTripDelay": "PT1M21.5530293S",
        "averageOutboundRoundTripDelay": "PT59.3598898S",
        "maximumInboundRoundTripDelay": "-PT3M23.0499547S",
        "maximumOutboundRoundTripDelay": "-PT1.4105079S",
        "averageInboundJitter": "-PT48.4657493S",
        "averageOutboundJitter": "PT1M12.8842618S",
        "maximumInboundJitter": "PT2M38.2625769S",
        "maximumOutboundJitter": "PT15.9549135S"
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

