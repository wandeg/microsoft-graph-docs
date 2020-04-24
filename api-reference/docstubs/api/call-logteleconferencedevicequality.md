---
title: "call: logTeleconferenceDeviceQuality"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# logTeleconferenceDeviceQuality

Namespace: microsoft.graph

**TODO: Add Description**

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

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
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|quality|[teleconferenceDeviceQuality](../resources/teleconferencedevicequality.md)|**TODO: Add Description**|



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

Content-Type: application/json
Content-length: 1811

{
  "quality": {
    "@odata.type": "microsoft.graph.teleconferenceDeviceQuality",
    "callChainId": "71a71673-1673-71a7-7316-a7717316a771",
    "participantId": "84a6abd5-abd5-84a6-d5ab-a684d5aba684",
    "mediaLegId": "b8d81e76-1e76-b8d8-761e-d8b8761ed8b8",
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
        "mediaDuration": "PT3M5.47694S",
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
        "averageInboundRoundTripDelay": "-PT2M24.5327467S",
        "averageOutboundRoundTripDelay": "PT6.9662036S",
        "maximumInboundRoundTripDelay": "-PT1M15.8253652S",
        "maximumOutboundRoundTripDelay": "PT33.3111114S",
        "averageInboundJitter": "-PT2M58.0817336S",
        "averageOutboundJitter": "PT1M45.6548548S",
        "maximumInboundJitter": "-PT2M14.6380335S",
        "maximumOutboundJitter": "PT1M54.3646124S"
      }
    ]
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

