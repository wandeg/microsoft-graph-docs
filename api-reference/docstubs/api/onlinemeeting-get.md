---
title: "Get onlineMeeting"
description: "Read the properties and relationships of an onlineMeeting object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get onlineMeeting

Namespace: microsoft.graph

Read the properties and relationships of an [onlineMeeting](../resources/onlinemeeting.md) object.

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
GET /me/onlineMeetings/{onlineMeetingId}
GET /app/onlineMeetings/{onlineMeetingId}
GET /communications/onlineMeetings/{onlineMeetingId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_onlinemeeting"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/onlineMeetings/{onlineMeetingId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlineMeeting"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.onlineMeeting",
    "id": "8c5883c3-83c3-8c58-c383-588cc383588c",
    "creationDateTime": "String (timestamp)",
    "startDateTime": "String (timestamp)",
    "endDateTime": "String (timestamp)",
    "canceledDateTime": "String (timestamp)",
    "expirationDateTime": "String (timestamp)",
    "entryExitAnnouncement": "Boolean",
    "joinUrl": "String",
    "subject": "String",
    "isCancelled": "Boolean",
    "participants": {
      "@odata.type": "microsoft.graph.meetingParticipants"
    },
    "isBroadcast": "Boolean",
    "accessLevel": "String",
    "capabilities": [
      "String"
    ],
    "audioConferencing": {
      "@odata.type": "microsoft.graph.audioConferencing"
    },
    "chatInfo": {
      "@odata.type": "microsoft.graph.chatInfo"
    },
    "videoTeleconferenceId": "String",
    "externalId": "String",
    "joinInformation": {
      "@odata.type": "microsoft.graph.itemBody"
    }
  }
}
```

