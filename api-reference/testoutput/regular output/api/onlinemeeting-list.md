---
title: "List onlineMeetings"
description: "List properties and relationships of the onlineMeeting objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List onlineMeetings

Namespace: microsoft.graph

List properties and relationships of the [onlineMeeting](../resources/onlinemeeting.md) objects.

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
GET /me/onlineMeetings
GET /communications/onlineMeetings
GET /users/{usersId}/onlineMeetings
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [onlineMeeting](../resources/onlinemeeting.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_onlinemeeting"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/onlineMeetings
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.onlinemeeting)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1849

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.onlineMeeting",
      "id": "78200008-0008-7820-0800-207808002078",
      "creationDateTime": "2016-12-31T23:59:03.7411042+03:00",
      "startDateTime": "2016-12-31T23:59:14.2230899+03:00",
      "endDateTime": "2016-12-31T23:57:11.7522995+03:00",
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
  ]
}
```

