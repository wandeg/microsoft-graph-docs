---
title: "List segments"
description: "Get the segments from the segments navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List segments

Get the segments from the segments navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /communications/callRecords/{callRecordId}/sessions/{sessionId}/segments
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [segment](../resources/segment.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_segment"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/communications/callRecords/{callRecordId}/sessions/{sessionId}/segments
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.callrecords.segment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4988

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.callRecords.segment",
      "id": "7d904a78-4a78-7d90-784a-907d784a907d",
      "startDateTime": "2017-01-01T00:03:15.6077862+03:00",
      "endDateTime": "2017-01-01T00:01:17.3856072+03:00",
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
              "averageJitter": "PT1M6.1191588S",
              "maxJitter": "-PT1M28.6559915S",
              "averagePacketLossRate": "Single",
              "maxPacketLossRate": "Single",
              "averageRatioOfConcealedSamples": "Single",
              "maxRatioOfConcealedSamples": "Single",
              "averageRoundTripTime": "-PT3M17.5707825S",
              "maxRoundTripTime": "PT1M32.6696096S",
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
              "averageAudioNetworkJitter": "-PT2M54.7666186S",
              "maxAudioNetworkJitter": "PT2.7210748S"
            }
          ]
        }
      ]
    }
  ]
}
```

