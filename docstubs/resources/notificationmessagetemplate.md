---
title: "notificationMessageTemplate resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# notificationMessageTemplate resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get notificationMessageTemplate](../api/notificationmessagetemplate-get.md)|[notificationMessageTemplate](../resources/notificationmessagetemplate.md)|Read properties and relationships of the [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object.|
|[Update notificationMessageTemplate](../api/notificationmessagetemplate-update.md)|[notificationMessageTemplate](../resources/notificationmessagetemplate.md)|Update the properties of a [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object.|
|[sendTestMessage](../api/notificationmessagetemplate-sendtestmessage.md)|None||
|[List localizedNotificationMessages](../api/notificationmessagetemplate-list-localizednotificationmessages.md)|[localizedNotificationMessage](../resources/localizednotificationmessage.md) collection|Get the localizedNotificationMessages from the localizedNotificationMessages navigation property.|
|[Add localizedNotificationMessages](../api/notificationmessagetemplate-post-localizednotificationmessages.md)|[localizedNotificationMessage](../resources/localizednotificationmessage.md)|Add localizedNotificationMessages by posting to the localizedNotificationMessages collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|brandingOptions|Enumeration| Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.|
|defaultLocale|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|roleScopeTagIds|String collection||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|localizedNotificationMessages|[localizedNotificationMessage](../resources/localizednotificationmessage.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.notificationMessageTemplate",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "defaultLocale": "String",
  "brandingOptions": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```

