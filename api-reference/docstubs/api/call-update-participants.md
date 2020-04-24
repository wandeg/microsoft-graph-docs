---
title: "Update participants"
description: "Update the properties of a participants object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update participants

Namespace: microsoft.graph

Update the properties of a participants object.

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
PATCH /communications/calls/{callId}/participants
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [participant](../resources/participant.md) object.

The following table shows the properties that are required when you create the [participant](../resources/participant.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|info|[participantInfo](../resources/participantinfo.md)|**TODO: Add Description**|
|recordingInfo|[recordingInfo](../resources/recordinginfo.md)|**TODO: Add Description**|
|mediaStreams|[mediaStream](../resources/mediastream.md) collection|**TODO: Add Description**|
|metadata|String|**TODO: Add Description**|
|isMuted|Boolean|**TODO: Add Description**|
|isInLobby|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [participant](../resources/participant.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_participants"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/communications/calls/{callId}/participants
Content-Type: application/json
Content-length: 1270

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
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
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
```

