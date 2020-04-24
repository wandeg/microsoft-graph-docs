---
title: "onlineMeeting: createOrGet"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# createOrGet

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /me/onlineMeetings/createOrGet
POST /app/onlineMeetings/createOrGet
POST /communications/onlineMeetings/createOrGet
POST /users/{usersId}/onlineMeetings/createOrGet
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|chatInfo|[chatInfo](../resources/chatinfo.md)|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|participants|[meetingParticipants](../resources/meetingparticipants.md)|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|



## Response
If successful, this action returns a `200 OK` response code and a [onlineMeeting](../resources/onlinemeeting.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "onlinemeeting_createorget"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/onlineMeetings/createOrGet

Content-Type: application/json
Content-length: 339

{
  "chatInfo": {
    "@odata.type": "microsoft.graph.chatInfo"
  },
  "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
  "externalId": "External Id value",
  "participants": {
    "@odata.type": "microsoft.graph.meetingParticipants"
  },
  "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
  "subject": "Subject value"
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

