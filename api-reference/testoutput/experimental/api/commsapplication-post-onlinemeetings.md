---
title: "Add onlineMeetings"
description: "Add onlineMeetings by posting to the onlineMeetings collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add onlineMeetings

Add onlineMeetings by posting to the onlineMeetings collection.

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
POST /app/onlineMeetings/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the onlineMeeting object.

The following table shows the properties that are required when you create the onlineMeeting.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|creationDateTime|DateTimeOffset||
|startDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||
|canceledDateTime|DateTimeOffset||
|expirationDateTime|DateTimeOffset||
|entryExitAnnouncement|Boolean||
|joinUrl|String||
|subject|String||
|isCancelled|Boolean||
|participants|[meetingParticipants](../resources/meetingParticipants.md)||
|isBroadcast|Boolean||
|accessLevel|Enumeration|. Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `sameEnterpriseAndFederated`.|
|capabilities|Enumeration collection|. Possible values are: `questionAndAnswer`, `unknownFutureValue`.|
|audioConferencing|[audioConferencing](../resources/audioConferencing.md)||
|chatInfo|[chatInfo](../resources/chatInfo.md)||
|videoTeleconferenceId|String||



## Response
If successful, this method returns a `201 Created` response code and a [onlineMeeting](../resources/onlinemeeting.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_onlinemeeting_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/app/onlineMeetings
Content-type: application/json
Content-length: 2075

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "creationDateTime": "2017-01-01T00:00:59.0982804+03:00",
  "startDateTime": "2017-01-01T00:03:15.6077862+03:00",
  "endDateTime": "2017-01-01T00:01:17.3856072+03:00",
  "canceledDateTime": "2016-12-31T23:59:04.935877+03:00",
  "expirationDateTime": "2017-01-01T00:01:09.280378+03:00",
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
  "videoTeleconferenceId": "Video Teleconference Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlinemeeting"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2124

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "id": "96cd02c9-02c9-96cd-c902-cd96c902cd96",
  "creationDateTime": "2017-01-01T00:00:59.0982804+03:00",
  "startDateTime": "2017-01-01T00:03:15.6077862+03:00",
  "endDateTime": "2017-01-01T00:01:17.3856072+03:00",
  "canceledDateTime": "2016-12-31T23:59:04.935877+03:00",
  "expirationDateTime": "2017-01-01T00:01:09.280378+03:00",
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
  "videoTeleconferenceId": "Video Teleconference Id value"
}
```

