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
|Authorization|Bearer {token}. Required|

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
    "id": "6362926d-926d-6362-6d92-62636d926263",
    "creationDateTime": "2016-12-31T23:59:05.697798+03:00",
    "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
    "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
    "canceledDateTime": "2017-01-01T00:01:30.7313696+03:00",
    "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
    "entryExitAnnouncement": true,
    "joinUrl": "https://example.com/joinUrl/",
    "subject": "Subject value",
    "isCancelled": true,
    "participants": {
      "@odata.type": "microsoft.graph.meetingParticipants",
      "organizer": {
        "@odata.type": "microsoft.graph.meetingParticipantInfo",
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
        "upn": "Upn value"
      },
      "attendees": [
        {
          "@odata.type": "microsoft.graph.meetingParticipantInfo"
        }
      ],
      "producers": [
        {
          "@odata.type": "microsoft.graph.meetingParticipantInfo"
        }
      ],
      "contributors": [
        {
          "@odata.type": "microsoft.graph.meetingParticipantInfo"
        }
      ]
    },
    "isBroadcast": true,
    "accessLevel": "String",
    "capabilities": [
      "String"
    ],
    "audioConferencing": {
      "@odata.type": "microsoft.graph.audioConferencing",
      "conferenceId": "Conference Id value",
      "tollNumber": "Toll Number value",
      "tollFreeNumber": "Toll Free Number value",
      "dialinUrl": "https://example.com/dialinUrl/"
    },
    "chatInfo": {
      "@odata.type": "microsoft.graph.chatInfo",
      "threadId": "Thread Id value",
      "messageId": "Message Id value",
      "replyChainMessageId": "Reply Chain Message Id value"
    },
    "videoTeleconferenceId": "Video Teleconference Id value",
    "externalId": "External Id value",
    "joinInformation": {
      "@odata.type": "microsoft.graph.itemBody",
      "contentType": "String",
      "content": "Content value"
    }
  }
}
```

