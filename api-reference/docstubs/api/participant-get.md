---
title: "Get participant"
description: "Read the properties and relationships of a participant object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get participant

Namespace: microsoft.graph

Read the properties and relationships of a [participant](../resources/participant.md) object.

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
GET /communications/calls/{callId}/participants/{participantId}
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
If successful, this method returns a `200 OK` response code and a [participant](../resources/participant.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_participant"
}
-->
``` http
GET https://graph.microsoft.com/beta/communications/calls/{callId}/participants/{participantId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.participant"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.participant",
    "id": "37eabbaa-bbaa-37ea-aabb-ea37aabbea37",
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
      },
      "initiator": {
        "@odata.type": "microsoft.graph.identitySet"
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
}
```

