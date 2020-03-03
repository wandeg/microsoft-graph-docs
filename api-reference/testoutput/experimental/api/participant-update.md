---
title: "Update participant"
description: "Update the properties of a participant object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update participant

Update the properties of a [participant](../resources/participant.md) object.

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
PATCH /communications/calls/{callId}/participants/{participantId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [participant](../resources/participant.md) object.

The following table shows the properties that are required when you create the [participant](../resources/participant.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|info|[participantInfo](../resources/participantInfo.md)||
|recordingInfo|[recordingInfo](../resources/recordingInfo.md)||
|mediaStreams|[mediaStream](../resources/mediaStream.md) collection||
|metadata|String||
|isMuted|Boolean||
|isInLobby|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [participant](../resources/participant.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_participant"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/communications/calls/{callId}/participants/{participantId}
Content-type: application/json
Content-length: 1190

{
  "@odata.type": "#microsoft.graph.participant",
  "info": {
    "@odata.type": "microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "id": "Id value",
        "displayName": "Display Name value"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "endpointType": "String",
    "region": "Region value",
    "languageId": "Language Id value",
    "countryCode": "Country Code value"
  },
  "recordingInfo": {
    "@odata.type": "microsoft.graph.recordingInfo",
    "recordingStatus": "String",
    "initiatedBy": {
      "@odata.type": "microsoft.graph.participantInfo"
    }
  },
  "mediaStreams": [
    {
      "@odata.type": "microsoft.graph.mediaStream",
      "mediaType": "String",
      "label": "Label value",
      "sourceId": "Source Id value",
      "direction": "String",
      "serverMuted": true
    }
  ],
  "metadata": "Metadata value",
  "isMuted": true,
  "isInLobby": true
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
Content-Length: 1239

{
  "@odata.type": "#microsoft.graph.participant",
  "id": "f57a5439-5439-f57a-3954-7af539547af5",
  "info": {
    "@odata.type": "microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "id": "Id value",
        "displayName": "Display Name value"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "endpointType": "String",
    "region": "Region value",
    "languageId": "Language Id value",
    "countryCode": "Country Code value"
  },
  "recordingInfo": {
    "@odata.type": "microsoft.graph.recordingInfo",
    "recordingStatus": "String",
    "initiatedBy": {
      "@odata.type": "microsoft.graph.participantInfo"
    }
  },
  "mediaStreams": [
    {
      "@odata.type": "microsoft.graph.mediaStream",
      "mediaType": "String",
      "label": "Label value",
      "sourceId": "Source Id value",
      "direction": "String",
      "serverMuted": true
    }
  ],
  "metadata": "Metadata value",
  "isMuted": true,
  "isInLobby": true
}
```

