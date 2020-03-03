---
title: "skypeForBusinessActivityUserDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# skypeForBusinessActivityUserDetail resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List skypeForBusinessActivityUserDetails](../api/skypeforbusinessactivityuserdetail-list.md)|[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md) collection|List properties and relationships of the [skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md) objects.|
|[Get skypeForBusinessActivityUserDetail](../api/skypeforbusinessactivityuserdetail-get.md)|[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)|Read properties and relationships of the [skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md) object.|
|[Create skypeForBusinessActivityUserDetail](../api/skypeforbusinessactivityuserdetail-create.md)|[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)|Create a new [skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md) object.|
|[Delete skypeForBusinessActivityUserDetail](../api/skypeforbusinessactivityuserdetail-delete.md)|None|Deletes a [skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md).|
|[Update skypeForBusinessActivityUserDetail](../api/skypeforbusinessactivityuserdetail-update.md)|[skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md)|Update the properties of a [skypeForBusinessActivityUserDetail](../resources/skypeforbusinessactivityuserdetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedProducts|String collection||
|deletedDate|Date||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean||
|lastActivityDate|Date||
|organizedConferenceAppSharingCount|Int64||
|organizedConferenceAudioVideoCount|Int64||
|organizedConferenceAudioVideoMinutes|Int64||
|organizedConferenceCloudDialInMicrosoftMinutes|Int64||
|organizedConferenceCloudDialInOutMicrosoftCount|Int64||
|organizedConferenceCloudDialOutMicrosoftMinutes|Int64||
|organizedConferenceDialInOut3rdPartyCount|Int64||
|organizedConferenceIMCount|Int64||
|organizedConferenceLastActivityDate|Date||
|organizedConferenceWebCount|Int64||
|participatedConferenceAppSharingCount|Int64||
|participatedConferenceAudioVideoCount|Int64||
|participatedConferenceAudioVideoMinutes|Int64||
|participatedConferenceDialInOut3rdPartyCount|Int64||
|participatedConferenceIMCount|Int64||
|participatedConferenceLastActivityDate|Date||
|participatedConferenceWebCount|Int64||
|peerToPeerAppSharingCount|Int64||
|peerToPeerAudioCount|Int64||
|peerToPeerAudioMinutes|Int64||
|peerToPeerFileTransferCount|Int64||
|peerToPeerIMCount|Int64||
|peerToPeerLastActivityDate|Date||
|peerToPeerVideoCount|Int64||
|peerToPeerVideoMinutes|Int64||
|reportPeriod|String||
|reportRefreshDate|Date||
|totalOrganizedConferenceCount|Int64||
|totalParticipatedConferenceCount|Int64||
|totalPeerToPeerSessionCount|Int64||
|userPrincipalName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeForBusinessActivityUserDetail",
  "id": "String (identifier)",
  "totalPeerToPeerSessionCount": 1024,
  "totalOrganizedConferenceCount": 1024,
  "totalParticipatedConferenceCount": 1024,
  "peerToPeerLastActivityDate": "Date",
  "organizedConferenceLastActivityDate": "Date",
  "participatedConferenceLastActivityDate": "Date",
  "peerToPeerIMCount": 1024,
  "peerToPeerAudioCount": 1024,
  "peerToPeerAudioMinutes": 1024,
  "peerToPeerVideoCount": 1024,
  "peerToPeerVideoMinutes": 1024,
  "peerToPeerAppSharingCount": 1024,
  "peerToPeerFileTransferCount": 1024,
  "organizedConferenceIMCount": 1024,
  "organizedConferenceAudioVideoCount": 1024,
  "organizedConferenceAudioVideoMinutes": 1024,
  "organizedConferenceAppSharingCount": 1024,
  "organizedConferenceWebCount": 1024,
  "organizedConferenceDialInOut3rdPartyCount": 1024,
  "organizedConferenceCloudDialInOutMicrosoftCount": 1024,
  "organizedConferenceCloudDialInMicrosoftMinutes": 1024,
  "organizedConferenceCloudDialOutMicrosoftMinutes": 1024,
  "participatedConferenceIMCount": 1024,
  "participatedConferenceAudioVideoCount": 1024,
  "participatedConferenceAudioVideoMinutes": 1024,
  "participatedConferenceAppSharingCount": 1024,
  "participatedConferenceWebCount": 1024,
  "participatedConferenceDialInOut3rdPartyCount": 1024,
  "reportRefreshDate": "Date",
  "userPrincipalName": "String",
  "isDeleted": true,
  "deletedDate": "Date",
  "lastActivityDate": "Date",
  "assignedProducts": [
    "String"
  ],
  "reportPeriod": "String"
}
```

