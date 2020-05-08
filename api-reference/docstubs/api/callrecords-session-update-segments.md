---
title: "Update segments"
description: "Update the properties of a segments object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update segments

Namespace: microsoft.graph.callRecords

Update the properties of a segments object.

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
PATCH /communications/callRecords/{callRecordId}/sessions/{sessionId}/segments
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [segment](../resources/callrecords-segment.md) object.

The following table shows the properties that are required when you create the [segment](../resources/callrecords-segment.md).

|Property|Type|Description|
|:---|:---|:---|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|caller|[endpoint](../resources/callrecords-endpoint.md)|**TODO: Add Description**|
|callee|[endpoint](../resources/callrecords-endpoint.md)|**TODO: Add Description**|
|failureInfo|[failureInfo](../resources/callrecords-failureinfo.md)|**TODO: Add Description**|
|media|[media](../resources/callrecords-media.md) collection|**TODO: Add Description**|
|id|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [segment](../resources/callrecords-segment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_segments"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/communications/callRecords/{callRecordId}/sessions/{sessionId}/segments
Content-Type: application/json
Content-length: 4461

{
  "@odata.type": "#microsoft.graph.callRecords.segment",
  "startDateTime": "2016-12-31T23:56:48.8437798+03:00",
  "endDateTime": "2016-12-31T23:57:13.0779697+03:00",
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
          "averageJitter": "-PT2M17.1009318S",
          "maxJitter": "-PT3M12.5607108S",
          "averagePacketLossRate": "Single",
          "maxPacketLossRate": "Single",
          "averageRatioOfConcealedSamples": "Single",
          "maxRatioOfConcealedSamples": "Single",
          "averageRoundTripTime": "PT3M0.6498984S",
          "maxRoundTripTime": "-PT45.933464S",
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
          "averageAudioNetworkJitter": "PT2M2.0456729S",
          "maxAudioNetworkJitter": "PT1M38.6292672S"
        }
      ]
    }
  ]
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
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.callRecords.segment",
  "startDateTime": "2016-12-31T23:56:48.8437798+03:00",
  "endDateTime": "2016-12-31T23:57:13.0779697+03:00",
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
          "averageJitter": "-PT2M17.1009318S",
          "maxJitter": "-PT3M12.5607108S",
          "averagePacketLossRate": "Single",
          "maxPacketLossRate": "Single",
          "averageRatioOfConcealedSamples": "Single",
          "maxRatioOfConcealedSamples": "Single",
          "averageRoundTripTime": "PT3M0.6498984S",
          "maxRoundTripTime": "-PT45.933464S",
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
          "averageAudioNetworkJitter": "PT2M2.0456729S",
          "maxAudioNetworkJitter": "PT1M38.6292672S"
        }
      ]
    }
  ],
  "id": "267fece5-ece5-267f-e5ec-7f26e5ec7f26"
}
```

