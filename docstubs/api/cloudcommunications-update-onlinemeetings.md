---
title: "Update onlineMeetings"
description: "Update the properties of an onlineMeetings object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update onlineMeetings

Namespace: microsoft.graph

Update the properties of an onlineMeetings object.

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
PATCH /communications/onlineMeetings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [onlineMeeting](../resources/onlinemeeting.md) object.

The following table shows the properties that are required when you create the [onlineMeeting](../resources/onlinemeeting.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|creationDateTime|DateTimeOffset|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|canceledDateTime|DateTimeOffset|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|entryExitAnnouncement|Boolean|**TODO: Add Description**|
|joinUrl|String|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|
|isCancelled|Boolean|**TODO: Add Description**|
|participants|[meetingParticipants](../resources/meetingparticipants.md)|**TODO: Add Description**|
|isBroadcast|Boolean|**TODO: Add Description**|
|accessLevel|accessLevel|**TODO: Add Description**. Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `sameEnterpriseAndFederated`.|
|capabilities|meetingCapabilities collection|**TODO: Add Description**. Possible values are: `questionAndAnswer`, `unknownFutureValue`.|
|audioConferencing|[audioConferencing](../resources/audioconferencing.md)|**TODO: Add Description**|
|chatInfo|[chatInfo](../resources/chatinfo.md)|**TODO: Add Description**|
|videoTeleconferenceId|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [onlineMeeting](../resources/onlinemeeting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_onlinemeetings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/communications/onlineMeetings
Content-Type: application/json
Content-length: 2077

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "creationDateTime": "2017-01-01T00:01:21.3942888+03:00",
  "startDateTime": "2017-01-01T00:03:24.4987822+03:00",
  "endDateTime": "2016-12-31T23:59:38.6819041+03:00",
  "canceledDateTime": "2017-01-01T00:02:45.1842181+03:00",
  "expirationDateTime": "2016-12-31T23:59:10.7331181+03:00",
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "id": "ad99b772-b772-ad99-72b7-99ad72b799ad",
  "creationDateTime": "2017-01-01T00:01:21.3942888+03:00",
  "startDateTime": "2017-01-01T00:03:24.4987822+03:00",
  "endDateTime": "2016-12-31T23:59:38.6819041+03:00",
  "canceledDateTime": "2017-01-01T00:02:45.1842181+03:00",
  "expirationDateTime": "2016-12-31T23:59:10.7331181+03:00",
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

