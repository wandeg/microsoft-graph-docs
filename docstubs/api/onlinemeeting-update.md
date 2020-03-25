---
title: "Update onlineMeeting"
description: "Update the properties of a onlineMeeting object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update onlineMeeting

Namespace: microsoft.graph

Update the properties of a [onlineMeeting](../resources/onlinemeeting.md) object.

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
PATCH /me/onlineMeetings/{onlineMeetingId}
PATCH /communications/onlineMeetings/{onlineMeetingId}
PATCH /users/{usersId}/onlineMeetings/{onlineMeetingId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [onlineMeeting](../resources/onlinemeeting.md) object.

The following table shows the properties that are required when you create the [onlineMeeting](../resources/onlinemeeting.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|creationDateTime|DateTimeOffset||
|startDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||
|joinUrl|String||
|subject|String||
|participants|[meetingParticipants](../resources/meetingparticipants.md)||
|audioConferencing|[audioConferencing](../resources/audioconferencing.md)||
|chatInfo|[chatInfo](../resources/chatinfo.md)||
|videoTeleconferenceId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [onlineMeeting](../resources/onlinemeeting.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_onlinemeeting"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/onlineMeetings/{onlineMeetingId}
Content-type: application/json
Content-length: 1579

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "creationDateTime": "2016-12-31T23:58:59.9945757+03:00",
  "startDateTime": "2017-01-01T00:01:40.4483143+03:00",
  "endDateTime": "2016-12-31T23:56:48.6937674+03:00",
  "joinUrl": "https://example.com/joinUrl/",
  "subject": "Subject value",
  "participants": {
    "@odata.type": "microsoft.graph.meetingParticipants",
    "organizer": {
      "@odata.type": "microsoft.graph.meetingParticipantInfo",
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
      "upn": "Upn value"
    },
    "attendees": [
      {
        "@odata.type": "microsoft.graph.meetingParticipantInfo"
      }
    ]
  },
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
  "videoTeleconferenceId": "Video Teleconference Id value"
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
Content-Length: 1628

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "id": "b97a035e-035e-b97a-5e03-7ab95e037ab9",
  "creationDateTime": "2016-12-31T23:58:59.9945757+03:00",
  "startDateTime": "2017-01-01T00:01:40.4483143+03:00",
  "endDateTime": "2016-12-31T23:56:48.6937674+03:00",
  "joinUrl": "https://example.com/joinUrl/",
  "subject": "Subject value",
  "participants": {
    "@odata.type": "microsoft.graph.meetingParticipants",
    "organizer": {
      "@odata.type": "microsoft.graph.meetingParticipantInfo",
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
      "upn": "Upn value"
    },
    "attendees": [
      {
        "@odata.type": "microsoft.graph.meetingParticipantInfo"
      }
    ]
  },
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
  "videoTeleconferenceId": "Video Teleconference Id value"
}
```

