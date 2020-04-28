---
title: "serviceUserAgent resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# serviceUserAgent resource type


Namespace: microsoft.graph.callRecords

**TODO: Add Description**


Inherits from [userAgent](../resources/useragent.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationVersion|String|**TODO: Add Description** Inherited from [userAgent](../resources/callrecords-useragent.md)|
|headerValue|String|**TODO: Add Description** Inherited from [userAgent](../resources/callrecords-useragent.md)|
|role|serviceRole|**TODO: Add Description**. Possible values are: `unknown`, `customBot`, `skypeForBusinessMicrosoftTeamsGateway`, `skypeForBusinessAudioVideoMcu`, `skypeForBusinessApplicationSharingMcu`, `skypeForBusinessCallQueues`, `skypeForBusinessAutoAttendant`, `mediationServer`, `mediationServerCloudConnectorEdition`, `exchangeUnifiedMessagingService`, `mediaController`, `conferencingAnnouncementService`, `conferencingAttendant`, `audioTeleconferencerController`, `skypeForBusinessUnifiedCommunicationApplicationPlatform`, `responseGroupServiceAnnouncementService`, `gateway`, `skypeTranslator`, `skypeForBusinessAttendant`, `responseGroupService`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.serviceUserAgent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.serviceUserAgent",
  "headerValue": "String",
  "applicationVersion": "String",
  "role": "String"
}
```

