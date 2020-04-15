---
title: "List onlineMeetings"
description: "Get the onlineMeetings from the onlineMeetings navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List onlineMeetings

Namespace: microsoft.graph

Get the onlineMeetings from the onlineMeetings navigation property.

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
GET /me/onlineMeetings
GET /users/{usersId}/onlineMeetings
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
If successful, this method returns a `200 OK` response code and a collection of [onlineMeeting](../resources/onlinemeeting.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_onlinemeeting"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/onlineMeetings
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.onlinemeeting)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.onlineMeeting",
      "id": "1e9325a2-25a2-1e93-a225-931ea225931e",
      "creationDateTime": "2016-12-31T23:59:20.5013691+03:00",
      "startDateTime": "2016-12-31T23:57:57.6528656+03:00",
      "endDateTime": "2016-12-31T23:58:04.9423402+03:00",
      "canceledDateTime": "2017-01-01T00:03:17.158695+03:00",
      "expirationDateTime": "2016-12-31T23:57:13.9832195+03:00",
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
  ]
}
```

