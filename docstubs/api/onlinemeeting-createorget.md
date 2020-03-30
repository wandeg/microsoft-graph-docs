---
title: "createOrGet"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# createOrGet

Namespace: microsoft.graph



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
POST /me/onlineMeetings/createOrGet
POST /app/onlineMeetings/createOrGet
POST /communications/onlineMeetings/createOrGet
POST /users/{usersId}/onlineMeetings/createOrGet
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|chatInfo|[chatInfo](../resources/chatinfo.md)||
|endDateTime|DateTimeOffset||
|externalId|String||
|participants|[meetingParticipants](../resources/meetingparticipants.md)||
|startDateTime|DateTimeOffset||
|subject|String||



## Response
If successful, this action returns a `200 OK` response code and a [onlineMeeting](../resources/onlinemeeting.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "onlinemeeting_createorget"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/onlineMeetings/createOrGet

Content-type: application/json
Content-length: 339

{
  "chatInfo": {
    "@odata.type": "microsoft.graph.chatInfo"
  },
  "endDateTime": "2017-01-01T00:01:31.3007329+03:00",
  "externalId": "External Id value",
  "participants": {
    "@odata.type": "microsoft.graph.meetingParticipants"
  },
  "startDateTime": "2017-01-01T00:01:00.4985153+03:00",
  "subject": "Subject value"
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
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1124

{
  "value": {
    "@odata.type": "#microsoft.graph.onlineMeeting",
    "id": "49f67c03-7c03-49f6-037c-f649037cf649",
    "creationDateTime": "2016-12-31T23:59:06.3080317+03:00",
    "startDateTime": "2017-01-01T00:01:00.4985153+03:00",
    "endDateTime": "2017-01-01T00:01:31.3007329+03:00",
    "canceledDateTime": "2016-12-31T23:59:12.8745008+03:00",
    "expirationDateTime": "2016-12-31T23:57:00.3383939+03:00",
    "entryExitAnnouncement": true,
    "joinUrl": "https://example.com/joinUrl/",
    "subject": "Subject value",
    "isCancelled": true,
    "participants": {
      "@odata.type": "microsoft.graph.meetingParticipants"
    },
    "isBroadcast": true,
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
    "videoTeleconferenceId": "Video Teleconference Id value",
    "externalId": "External Id value",
    "joinInformation": {
      "@odata.type": "microsoft.graph.itemBody"
    }
  }
}
```

