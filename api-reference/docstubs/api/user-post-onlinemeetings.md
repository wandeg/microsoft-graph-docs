---
title: "Create onlineMeetings"
description: "Create a new onlineMeetings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create onlineMeetings

Namespace: microsoft.graph

Create a new onlineMeetings object.

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
POST /me/onlineMeetings
POST /users/{usersId}/onlineMeetings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [onlineMeeting](../resources/onlinemeeting.md) object.

The following table shows the properties that are required when you create the [onlineMeeting](../resources/onlinemeeting.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|creationDateTime|DateTimeOffset|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|joinUrl|String|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|
|participants|[meetingParticipants](../resources/meetingparticipants.md)|**TODO: Add Description**|
|audioConferencing|[audioConferencing](../resources/audioconferencing.md)|**TODO: Add Description**|
|chatInfo|[chatInfo](../resources/chatinfo.md)|**TODO: Add Description**|
|videoTeleconferenceId|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [onlineMeeting](../resources/onlinemeeting.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_onlinemeeting_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/onlineMeetings
Content-Type: application/json
Content-length: 1579

{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "creationDateTime": "2017-01-01T00:00:16.3720534+03:00",
  "startDateTime": "2017-01-01T00:02:21.5483474+03:00",
  "endDateTime": "2016-12-31T23:57:31.2684087+03:00",
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onlinemeeting"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "id": "0a89f2c5-f2c5-0a89-c5f2-890ac5f2890a",
  "creationDateTime": "2017-01-01T00:00:16.3720534+03:00",
  "startDateTime": "2017-01-01T00:02:21.5483474+03:00",
  "endDateTime": "2016-12-31T23:57:31.2684087+03:00",
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

