---
title: "Update segment"
description: "Update the properties of a segment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update segment

Namespace: microsoft.graph.callRecords

Update the properties of a [segment](../resources/callrecords-segment.md) object.

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
PATCH /communications/callRecords/{callRecordId}/sessions/{sessionId}/segments/{segmentId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [segment](../resources/callrecords-segment.md) object.

The following table shows the properties that are required when you create the [segment](../resources/callrecords-segment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/callrecords-entity.md)|
|startDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||
|caller|[endpoint](../resources/callrecords-endpoint.md)||
|callee|[endpoint](../resources/callrecords-endpoint.md)||
|failureInfo|[failureInfo](../resources/callrecords-failureinfo.md)||
|media|[media](../resources/callrecords-media.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [segment](../resources/callrecords-segment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_segment"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/communications/callRecords/{callRecordId}/sessions/{sessionId}/segments/{segmentId}
Content-type: application/json
Content-length: 4460

{
  "@odata.type": "#microsoft.graph.callRecords.segment",
  "startDateTime": "2017-01-01T00:00:14.2767228+03:00",
  "endDateTime": "2017-01-01T00:02:18.392989+03:00",
  "caller": {
    "@odata.type": "microsoft.graph.callRecords.endpoint",
    "userAgent": {
      "@odata.type": "microsoft.graph.callRecords.userAgent",
      "headerValue": "Header Value value",
      "applicationVersion": "Application Version value"
    }
  },
  "callee": {
    "@odata.type": "microsoft.graph.callRecords.endpoint"
  },
  "failureInfo": {
    "@odata.type": "microsoft.graph.callRecords.failureInfo",
    "stage": "String",
    "reason": "Reason value"
  },
  "media": [
    {
      "@odata.type": "microsoft.graph.callRecords.media",
      "label": "Label value",
      "callerNetwork": {
        "@odata.type": "microsoft.graph.callRecords.networkInfo",
        "ipAddress": "Ip Address value",
        "subnet": "Subnet value",
        "linkSpeed": 9,
        "connectionType": "String",
        "port": 4,
        "reflexiveIPAddress": "Reflexive IPAddress value",
        "relayIPAddress": "Relay IPAddress value",
        "relayPort": 9,
        "macAddress": "Mac Address value",
        "wifiMicrosoftDriver": "Wifi Microsoft Driver value",
        "wifiMicrosoftDriverVersion": "Wifi Microsoft Driver Version value",
        "wifiVendorDriver": "Wifi Vendor Driver value",
        "wifiVendorDriverVersion": "Wifi Vendor Driver Version value",
        "wifiChannel": 11,
        "wifiBand": "String",
        "basicServiceSetIdentifier": "Basic Service Set Identifier value",
        "wifiRadioType": "String",
        "wifiSignalStrength": 2,
        "wifiBatteryCharge": 1,
        "dnsSuffix": "Dns Suffix value",
        "sentQualityEventRatio": "Single",
        "receivedQualityEventRatio": "Single",
        "delayEventRatio": "Single",
        "bandwidthLowEventRatio": "Single"
      },
      "calleeNetwork": {
        "@odata.type": "microsoft.graph.callRecords.networkInfo"
      },
      "callerDevice": {
        "@odata.type": "microsoft.graph.callRecords.deviceInfo",
        "captureDeviceName": "Capture Device Name value",
        "captureDeviceDriver": "Capture Device Driver value",
        "renderDeviceName": "Render Device Name value",
        "renderDeviceDriver": "Render Device Driver value",
        "sentSignalLevel": 15,
        "receivedSignalLevel": 3,
        "sentNoiseLevel": 14,
        "receivedNoiseLevel": 2,
        "initialSignalLevelRootMeanSquare": "Single",
        "cpuInsufficentEventRatio": "Single",
        "renderNotFunctioningEventRatio": "Single",
        "captureNotFunctioningEventRatio": "Single",
        "deviceGlitchEventRatio": "Single",
        "lowSpeechToNoiseEventRatio": "Single",
        "lowSpeechLevelEventRatio": "Single",
        "deviceClippingEventRatio": "Single",
        "howlingEventCount": 1,
        "renderZeroVolumeEventRatio": "Single",
        "renderMuteEventRatio": "Single",
        "micGlitchRate": "Single",
        "speakerGlitchRate": "Single"
      },
      "calleeDevice": {
        "@odata.type": "microsoft.graph.callRecords.deviceInfo"
      },
      "streams": [
        {
          "@odata.type": "microsoft.graph.callRecords.mediaStream",
          "streamId": "Stream Id value",
          "streamDirection": "String",
          "averageAudioDegradation": "Single",
          "averageJitter": "PT2M0.8921439S",
          "maxJitter": "PT39.3885375S",
          "averagePacketLossRate": "Single",
          "maxPacketLossRate": "Single",
          "averageRatioOfConcealedSamples": "Single",
          "maxRatioOfConcealedSamples": "Single",
          "averageRoundTripTime": "-PT1M49.1540522S",
          "maxRoundTripTime": "-PT43.6832843S",
          "packetUtilization": 1,
          "averageBandwidthEstimate": 8,
          "wasMediaBypassed": true,
          "postForwardErrorCorrectionPacketLossRate": "Single",
          "averageVideoFrameLossPercentage": "Single",
          "averageReceivedFrameRate": "Single",
          "lowFrameRateRatio": "Single",
          "averageVideoPacketLossRate": "Single",
          "averageVideoFrameRate": "Single",
          "lowVideoProcessingCapabilityRatio": "Single",
          "averageAudioNetworkJitter": "-PT1M13.422285S",
          "maxAudioNetworkJitter": "-PT3M15.7657564S"
        }
      ]
    }
  ]
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
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4509

{
  "@odata.type": "#microsoft.graph.callRecords.segment",
  "id": "43fd3a1b-3a1b-43fd-1b3a-fd431b3afd43",
  "startDateTime": "2017-01-01T00:00:14.2767228+03:00",
  "endDateTime": "2017-01-01T00:02:18.392989+03:00",
  "caller": {
    "@odata.type": "microsoft.graph.callRecords.endpoint",
    "userAgent": {
      "@odata.type": "microsoft.graph.callRecords.userAgent",
      "headerValue": "Header Value value",
      "applicationVersion": "Application Version value"
    }
  },
  "callee": {
    "@odata.type": "microsoft.graph.callRecords.endpoint"
  },
  "failureInfo": {
    "@odata.type": "microsoft.graph.callRecords.failureInfo",
    "stage": "String",
    "reason": "Reason value"
  },
  "media": [
    {
      "@odata.type": "microsoft.graph.callRecords.media",
      "label": "Label value",
      "callerNetwork": {
        "@odata.type": "microsoft.graph.callRecords.networkInfo",
        "ipAddress": "Ip Address value",
        "subnet": "Subnet value",
        "linkSpeed": 9,
        "connectionType": "String",
        "port": 4,
        "reflexiveIPAddress": "Reflexive IPAddress value",
        "relayIPAddress": "Relay IPAddress value",
        "relayPort": 9,
        "macAddress": "Mac Address value",
        "wifiMicrosoftDriver": "Wifi Microsoft Driver value",
        "wifiMicrosoftDriverVersion": "Wifi Microsoft Driver Version value",
        "wifiVendorDriver": "Wifi Vendor Driver value",
        "wifiVendorDriverVersion": "Wifi Vendor Driver Version value",
        "wifiChannel": 11,
        "wifiBand": "String",
        "basicServiceSetIdentifier": "Basic Service Set Identifier value",
        "wifiRadioType": "String",
        "wifiSignalStrength": 2,
        "wifiBatteryCharge": 1,
        "dnsSuffix": "Dns Suffix value",
        "sentQualityEventRatio": "Single",
        "receivedQualityEventRatio": "Single",
        "delayEventRatio": "Single",
        "bandwidthLowEventRatio": "Single"
      },
      "calleeNetwork": {
        "@odata.type": "microsoft.graph.callRecords.networkInfo"
      },
      "callerDevice": {
        "@odata.type": "microsoft.graph.callRecords.deviceInfo",
        "captureDeviceName": "Capture Device Name value",
        "captureDeviceDriver": "Capture Device Driver value",
        "renderDeviceName": "Render Device Name value",
        "renderDeviceDriver": "Render Device Driver value",
        "sentSignalLevel": 15,
        "receivedSignalLevel": 3,
        "sentNoiseLevel": 14,
        "receivedNoiseLevel": 2,
        "initialSignalLevelRootMeanSquare": "Single",
        "cpuInsufficentEventRatio": "Single",
        "renderNotFunctioningEventRatio": "Single",
        "captureNotFunctioningEventRatio": "Single",
        "deviceGlitchEventRatio": "Single",
        "lowSpeechToNoiseEventRatio": "Single",
        "lowSpeechLevelEventRatio": "Single",
        "deviceClippingEventRatio": "Single",
        "howlingEventCount": 1,
        "renderZeroVolumeEventRatio": "Single",
        "renderMuteEventRatio": "Single",
        "micGlitchRate": "Single",
        "speakerGlitchRate": "Single"
      },
      "calleeDevice": {
        "@odata.type": "microsoft.graph.callRecords.deviceInfo"
      },
      "streams": [
        {
          "@odata.type": "microsoft.graph.callRecords.mediaStream",
          "streamId": "Stream Id value",
          "streamDirection": "String",
          "averageAudioDegradation": "Single",
          "averageJitter": "PT2M0.8921439S",
          "maxJitter": "PT39.3885375S",
          "averagePacketLossRate": "Single",
          "maxPacketLossRate": "Single",
          "averageRatioOfConcealedSamples": "Single",
          "maxRatioOfConcealedSamples": "Single",
          "averageRoundTripTime": "-PT1M49.1540522S",
          "maxRoundTripTime": "-PT43.6832843S",
          "packetUtilization": 1,
          "averageBandwidthEstimate": 8,
          "wasMediaBypassed": true,
          "postForwardErrorCorrectionPacketLossRate": "Single",
          "averageVideoFrameLossPercentage": "Single",
          "averageReceivedFrameRate": "Single",
          "lowFrameRateRatio": "Single",
          "averageVideoPacketLossRate": "Single",
          "averageVideoFrameRate": "Single",
          "lowVideoProcessingCapabilityRatio": "Single",
          "averageAudioNetworkJitter": "-PT1M13.422285S",
          "maxAudioNetworkJitter": "-PT3M15.7657564S"
        }
      ]
    }
  ]
}
```

