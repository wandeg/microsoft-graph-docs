---
title: "Create skypeForBusinessActivityUserDetail"
description: "Create a new skypeForBusinessActivityUserDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create skypeForBusinessActivityUserDetail

Create a new [skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md) object.

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
POST ** Collection URI for microsoft.graph.skypeForBusinessActivityUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the skypeForBusinessActivityUserDetail object.

The following table shows the properties that are required when you create the skypeForBusinessActivityUserDetail.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|totalPeerToPeerSessionCount|Int64||
|totalOrganizedConferenceCount|Int64||
|totalParticipatedConferenceCount|Int64||
|peerToPeerLastActivityDate|Date||
|organizedConferenceLastActivityDate|Date||
|participatedConferenceLastActivityDate|Date||
|peerToPeerIMCount|Int64||
|peerToPeerAudioCount|Int64||
|peerToPeerAudioMinutes|Int64||
|peerToPeerVideoCount|Int64||
|peerToPeerVideoMinutes|Int64||
|peerToPeerAppSharingCount|Int64||
|peerToPeerFileTransferCount|Int64||
|organizedConferenceIMCount|Int64||
|organizedConferenceAudioVideoCount|Int64||
|organizedConferenceAudioVideoMinutes|Int64||
|organizedConferenceAppSharingCount|Int64||
|organizedConferenceWebCount|Int64||
|organizedConferenceDialInOut3rdPartyCount|Int64||
|organizedConferenceCloudDialInOutMicrosoftCount|Int64||
|organizedConferenceCloudDialInMicrosoftMinutes|Int64||
|organizedConferenceCloudDialOutMicrosoftMinutes|Int64||
|participatedConferenceIMCount|Int64||
|participatedConferenceAudioVideoCount|Int64||
|participatedConferenceAudioVideoMinutes|Int64||
|participatedConferenceAppSharingCount|Int64||
|participatedConferenceWebCount|Int64||
|participatedConferenceDialInOut3rdPartyCount|Int64||
|reportRefreshDate|Date||
|userPrincipalName|String||
|isDeleted|Boolean||
|deletedDate|Date||
|lastActivityDate|Date||
|assignedProducts|String collection||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_skypeforbusinessactivityuserdetail_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.skypeForBusinessActivityUserDetail not found
Content-type: application/json
Content-length: 1544

{
  "@odata.type": "#microsoft.graph.skypeForBusinessActivityUserDetail",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeforbusinessactivityuserdetail"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1593

{
  "@odata.type": "#microsoft.graph.skypeForBusinessActivityUserDetail",
  "id": "dcefb9cd-b9cd-dcef-cdb9-efdccdb9efdc",
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
```

