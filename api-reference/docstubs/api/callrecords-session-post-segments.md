---
title: "Create segments"
description: "Create a new segments object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create segments

Namespace: microsoft.graph.callRecords

Create a new segments object.

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
POST /communications/callRecords/{callRecordId}/sessions/{sessionId}/segments
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [segment](../resources/callrecords-segment.md) object.

The following table shows the properties that are required when you create the [segment](../resources/callrecords-segment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/callrecords-entity.md)|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|caller|[endpoint](../resources/callrecords-endpoint.md)|**TODO: Add Description**|
|callee|[endpoint](../resources/callrecords-endpoint.md)|**TODO: Add Description**|
|failureInfo|[failureInfo](../resources/callrecords-failureinfo.md)|**TODO: Add Description**|
|media|[media](../resources/callrecords-media.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [segment](../resources/callrecords-segment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_segment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/communications/callRecords/{callRecordId}/sessions/{sessionId}/segments
Content-Type: application/json
Content-length: 4464

{
  "@odata.type": "#microsoft.graph.callRecords.segment",
  "startDateTime": "2016-12-31T23:56:29.9610061+03:00",
  "endDateTime": "2017-01-01T00:00:21.2863747+03:00",
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
          "averageJitter": "PT2M20.6389308S",
          "maxJitter": "-PT2M58.3390431S",
          "averagePacketLossRate": "Single",
          "maxPacketLossRate": "Single",
          "averageRatioOfConcealedSamples": "Single",
          "maxRatioOfConcealedSamples": "Single",
          "averageRoundTripTime": "-PT1M26.763867S",
          "maxRoundTripTime": "-PT3M7.8988681S",
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
          "averageAudioNetworkJitter": "PT3M4.8834863S",
          "maxAudioNetworkJitter": "-PT3M16.9219793S"
        }
      ]
    }
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.callrecords.segment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.callRecords.segment",
  "id": "dab97368-7368-dab9-6873-b9da6873b9da",
  "startDateTime": "2016-12-31T23:56:29.9610061+03:00",
  "endDateTime": "2017-01-01T00:00:21.2863747+03:00",
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
          "averageJitter": "PT2M20.6389308S",
          "maxJitter": "-PT2M58.3390431S",
          "averagePacketLossRate": "Single",
          "maxPacketLossRate": "Single",
          "averageRatioOfConcealedSamples": "Single",
          "maxRatioOfConcealedSamples": "Single",
          "averageRoundTripTime": "-PT1M26.763867S",
          "maxRoundTripTime": "-PT3M7.8988681S",
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
          "averageAudioNetworkJitter": "PT3M4.8834863S",
          "maxAudioNetworkJitter": "-PT3M16.9219793S"
        }
      ]
    }
  ]
}
```

