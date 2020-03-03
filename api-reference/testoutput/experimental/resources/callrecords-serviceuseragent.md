---
title: "serviceUserAgent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph.callRecords
---


# serviceUserAgent resource type




Inherits from [userAgent](../resources/userAgent.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationVersion|String| Inherited from [userAgent](../resources/callRecords-userAgent.md)|
|headerValue|String| Inherited from [userAgent](../resources/callRecords-userAgent.md)|
|role|Enumeration|. Possible values are: `unknown`, `customBot`, `skypeForBusinessMicrosoftTeamsGateway`, `skypeForBusinessAudioVideoMcu`, `skypeForBusinessApplicationSharingMcu`, `skypeForBusinessCallQueues`, `skypeForBusinessAutoAttendant`, `mediationServer`, `mediationServerCloudConnectorEdition`, `exchangeUnifiedMessagingService`, `mediaController`, `conferencingAnnouncementService`, `conferencingAttendant`, `audioTeleconferencerController`, `skypeForBusinessUnifiedCommunicationApplicationPlatform`, `responseGroupServiceAnnouncementService`, `gateway`, `skypeTranslator`, `skypeForBusinessAttendant`, `responseGroupService`, `unknownFutureValue`.|

## Relationships
None

## JSON Representation
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

