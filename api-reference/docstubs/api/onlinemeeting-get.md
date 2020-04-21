---
title: "Get onlineMeeting"
description: "Read properties and relationships of an onlineMeeting object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get onlineMeeting

Namespace: microsoft.graph

Read properties and relationships of an [onlineMeeting](../resources/onlinemeeting.md) object.

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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
    "id": "2b16c17c-c17c-2b16-7cc1-162b7cc1162b",
    "creationDateTime": "2016-12-31T23:58:44.3655181+00:00",
    "startDateTime": "2016-12-31T23:57:14.5036527+00:00",
    "endDateTime": "2017-01-01T00:03:14.3547611+00:00",
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
}
```

