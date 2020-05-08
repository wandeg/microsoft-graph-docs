---
title: "List segments"
description: "Get the segments from the segments navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List segments

Namespace: microsoft.graph.callRecords

Get the segments from the segments navigation property.

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
GET /communications/callRecords/{callRecordId}/sessions/{sessionId}/segments
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [segment](../resources/segment.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_segment"
}
-->
``` http
GET https://graph.microsoft.com/beta/communications/callRecords/{callRecordId}/sessions/{sessionId}/segments
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.callrecords.segment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

