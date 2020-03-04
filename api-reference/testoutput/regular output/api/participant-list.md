---
title: "List participants"
description: "List properties and relationships of the participant objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List participants

Namespace: microsoft.graph

List properties and relationships of the [participant](../resources/participant.md) objects.

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
GET /communications/calls/{callId}/participants
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [participant](../resources/participant.md) objects in the response body.

## Example

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
Content-Length: 1098

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.participant",
      "id": "e619f90d-f90d-e619-0df9-19e60df919e6",
      "info": {
        "@odata.type": "microsoft.graph.participantInfo",
        "identity": {
          "@odata.type": "microsoft.graph.identitySet",
          "application": {
            "@odata.type": "microsoft.graph.identity",
            "displayName": "Display Name value",
            "id": "Id value"
          },
          "device": {
            "@odata.type": "microsoft.graph.identity"
          },
          "user": {
            "@odata.type": "microsoft.graph.identity"
          }
        },
        "region": "Region value",
        "languageId": "Language Id value"
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
      "isMuted": true,
      "isInLobby": true
    }
  ]
}
```

