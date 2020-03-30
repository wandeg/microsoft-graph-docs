---
title: "getSkypeForBusinessActivityUserDetail"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getSkypeForBusinessActivityUserDetail

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
GET /reports/getSkypeForBusinessActivityUserDetail
GET /print/reports/{reportRootId}/getSkypeForBusinessActivityUserDetail
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|period|String||



## Response
If successful, this function returns a `200 OK` response code and a [skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserDetail(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.skypeforbusinessactivityuserdetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1782

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.skypeForBusinessActivityUserDetail",
      "id": "7a365dde-5dde-7a36-de5d-367ade5d367a",
      "totalPeerToPeerSessionCount": 11,
      "totalOrganizedConferenceCount": 13,
      "totalParticipatedConferenceCount": 0,
      "peerToPeerLastActivityDate": "Date",
      "organizedConferenceLastActivityDate": "Date",
      "participatedConferenceLastActivityDate": "Date",
      "peerToPeerIMCount": 1,
      "peerToPeerAudioCount": 4,
      "peerToPeerAudioMinutes": 6,
      "peerToPeerVideoCount": 4,
      "peerToPeerVideoMinutes": 6,
      "peerToPeerAppSharingCount": 9,
      "peerToPeerFileTransferCount": 11,
      "organizedConferenceIMCount": 10,
      "organizedConferenceAudioVideoCount": 2,
      "organizedConferenceAudioVideoMinutes": 4,
      "organizedConferenceAppSharingCount": 2,
      "organizedConferenceWebCount": 11,
      "organizedConferenceDialInOut3rdPartyCount": 9,
      "organizedConferenceCloudDialInOutMicrosoftCount": 15,
      "organizedConferenceCloudDialInMicrosoftMinutes": 14,
      "organizedConferenceCloudDialOutMicrosoftMinutes": 15,
      "participatedConferenceIMCount": 13,
      "participatedConferenceAudioVideoCount": 5,
      "participatedConferenceAudioVideoMinutes": 7,
      "participatedConferenceAppSharingCount": 5,
      "participatedConferenceWebCount": 14,
      "participatedConferenceDialInOut3rdPartyCount": 12,
      "reportRefreshDate": "Date",
      "userPrincipalName": "User Principal Name value",
      "isDeleted": true,
      "deletedDate": "Date",
      "lastActivityDate": "Date",
      "assignedProducts": [
        "Assigned Products value"
      ],
      "reportPeriod": "Report Period value"
    }
  ]
}
```

