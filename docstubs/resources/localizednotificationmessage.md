---
title: "localizedNotificationMessage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# localizedNotificationMessage resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get localizedNotificationMessage](../api/localizednotificationmessage-get.md)|[localizedNotificationMessage](../resources/localizednotificationmessage.md)|Read properties and relationships of the [localizedNotificationMessage](../resources/localizednotificationmessage.md) object.|
|[Update localizedNotificationMessage](../api/localizednotificationmessage-update.md)|[localizedNotificationMessage](../resources/localizednotificationmessage.md)|Update the properties of a [localizedNotificationMessage](../resources/localizednotificationmessage.md) object.|
|[List localizedNotificationMessages](../api/notificationmessagetemplate-list-localizednotificationmessages.md)|[localizedNotificationMessage](../resources/localizednotificationmessage.md) collection|Get the localizedNotificationMessages from the localizedNotificationMessages navigation property.|
|[Add localizedNotificationMessages](../api/notificationmessagetemplate-post-localizednotificationmessages.md)|[localizedNotificationMessage](../resources/localizednotificationmessage.md)|Add localizedNotificationMessages by posting to the localizedNotificationMessages collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean||
|lastModifiedDateTime|DateTimeOffset||
|locale|String||
|messageTemplate|String||
|subject|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.localizedNotificationMessage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "locale": "String",
  "subject": "String",
  "messageTemplate": "String",
  "isDefault": true
}
```

