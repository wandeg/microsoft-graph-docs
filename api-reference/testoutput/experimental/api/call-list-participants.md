---
title: "List participants"
description: "Get the participants from the participants navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List participants

Namespace: microsoft.graph

Get the participants from the participants navigation property.

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
GET /communications/calls/{callId}/participants
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [participant](../resources/participant.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_participant"
}
-->
``` http
GET https://graph.microsoft.com/localtest/communications/calls/{callId}/participants
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.participant)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1444

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.participant",
      "id": "eba031f3-31f3-eba0-f331-a0ebf331a0eb",
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
  ]
}
```

