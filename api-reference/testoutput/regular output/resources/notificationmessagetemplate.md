---
title: "notificationMessageTemplate resource type"
description: "Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator. Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section. Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# notificationMessageTemplate resource type

Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator. Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section. Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get notificationMessageTemplate](../api/notificationmessagetemplate-get.md)|[notificationMessageTemplate](../resources/notificationMessageTemplate.md)|Read properties and relationships of the [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object.|
|[Delete notificationMessageTemplate](../api/notificationmessagetemplate-delete.md)|None|Deletes a [notificationMessageTemplate](../resources/notificationmessagetemplate.md).|
|[Update notificationMessageTemplate](../api/notificationmessagetemplate-update.md)|[notificationMessageTemplate](../resources/notificationMessageTemplate.md)|Update the properties of a [notificationMessageTemplate](../resources/notificationmessagetemplate.md) object.|
|[sendTestMessage](../api/notificationmessagetemplate-sendtestmessage.md)|None||
|[List localizedNotificationMessages](../api/notificationmessagetemplate-list-localizednotificationmessages.md)|[localizedNotificationMessage](../resources/localizedNotificationMessage.md) collection|Get the localizedNotificationMessages from the localizedNotificationMessages navigation property.|
|[Add localizedNotificationMessages](../api/notificationmessagetemplate-post-localizednotificationmessages.md)|[localizedNotificationMessage](../resources/localizedNotificationMessage.md)|Add localizedNotificationMessages by posting to the localizedNotificationMessages collection.|
|[List notificationMessageTemplates](../api/devicemanagement-list-notificationmessagetemplates.md)|[notificationMessageTemplate](../resources/notificationMessageTemplate.md) collection|Get the notificationMessageTemplates from the notificationMessageTemplates navigation property.|
|[Add notificationMessageTemplates](../api/devicemanagement-post-notificationmessagetemplates.md)|[notificationMessageTemplate](../resources/notificationMessageTemplate.md)|Add notificationMessageTemplates by posting to the notificationMessageTemplates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|brandingOptions|Enumeration|The Message Template Branding Options. Branding is defined in the Intune Admin Console. Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.|
|defaultLocale|String|The default locale to fallback onto when the requested locale is not available.|
|displayName|String|Display name for the Notification Message Template.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|localizedNotificationMessages|[localizedNotificationMessage](../resources/localizedNotificationMessage.md) collection|The list of localized messages for this Notification Message Template.|

## JSON Representation
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
  "brandingOptions": "String"
}
```

