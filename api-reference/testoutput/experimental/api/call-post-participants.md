---
title: "Add participants"
description: "Add participants by posting to the participants collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add participants

Namespace: microsoft.graph

Add participants by posting to the participants collection.

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
POST /communications/calls/{callId}/participants/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [participant](../resources/participant.md) object.

The following table shows the properties that are required when you create the [participant](../resources/participant.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|info|[participantInfo](../resources/participantinfo.md)||
|recordingInfo|[recordingInfo](../resources/recordinginfo.md)||
|mediaStreams|[mediaStream](../resources/mediastream.md) collection||
|metadata|String||
|isMuted|Boolean||
|isInLobby|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [participant](../resources/participant.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_participant_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/communications/calls/{callId}/participants
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
  "truncated": true,
  "@odata.type": "microsoft.graph.participant"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1239

{
  "@odata.type": "#microsoft.graph.participant",
  "id": "bcf70126-0126-bcf7-2601-f7bc2601f7bc",
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

