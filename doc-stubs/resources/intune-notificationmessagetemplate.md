---
title: "notificationMessageTemplate resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# notificationMessageTemplate resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List notificationMessageTemplates](../api/intune-devicemanagement-list-notificationmessagetemplates.md)|[notificationMessageTemplate](../resources/intune-notificationmessagetemplate.md) collection|Get the notificationMessageTemplates from the notificationMessageTemplates navigation property.|
|[Create notificationMessageTemplates](../api/intune-devicemanagement-post-notificationmessagetemplates.md)|[notificationMessageTemplate](../resources/intune-notificationmessagetemplate.md)|Create a new notificationMessageTemplates object.|
|[Delete notificationMessageTemplates](../api/intune-devicemanagement-delete-notificationmessagetemplates.md)|None|Delete a [notificationMessageTemplate](../resources/intune-notificationmessagetemplate.md) object.|
|[Update notificationMessageTemplates](../api/intune-devicemanagement-update-notificationmessagetemplates.md)|[notificationMessageTemplate](../resources/intune-notificationmessagetemplate.md)|Update the properties of a notificationMessageTemplates object.|
|[Get notificationMessageTemplates](../api/intune-devicemanagement-get-notificationmessagetemplate.md)|[notificationMessageTemplate](../resources/intune-notificationmessagetemplate.md)|Read the properties and relationships of a [notificationMessageTemplate](../resources/intune-notificationmessagetemplate.md) object.|
|[sendTestMessage](../api/intune-notificationmessagetemplate-sendtestmessage.md)|None|**TODO: Add Description**|
|[List localizedNotificationMessages](../api/intune-notificationmessagetemplate-list-localizednotificationmessages.md)|[localizedNotificationMessage](../resources/intune-localizednotificationmessage.md) collection|Get the localizedNotificationMessages from the localizedNotificationMessages navigation property.|
|[Create localizedNotificationMessages](../api/intune-notificationmessagetemplate-post-localizednotificationmessages.md)|[localizedNotificationMessage](../resources/intune-localizednotificationmessage.md)|Create a new localizedNotificationMessages object.|
|[Delete localizedNotificationMessages](../api/intune-notificationmessagetemplate-delete-localizednotificationmessages.md)|None|Delete a [localizedNotificationMessage](../resources/intune-localizednotificationmessage.md) object.|
|[Update localizedNotificationMessages](../api/intune-notificationmessagetemplate-update-localizednotificationmessages.md)|[localizedNotificationMessage](../resources/intune-localizednotificationmessage.md)|Update the properties of a localizedNotificationMessages object.|
|[Get localizedNotificationMessages](../api/intune-notificationmessagetemplate-get-localizednotificationmessage.md)|[localizedNotificationMessage](../resources/intune-localizednotificationmessage.md)|Read the properties and relationships of a [localizedNotificationMessage](../resources/intune-localizednotificationmessage.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|brandingOptions|notificationTemplateBrandingOptions|**TODO: Add Description**. Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.|
|defaultLocale|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|localizedNotificationMessages|[localizedNotificationMessage](../resources/intune-localizednotificationmessage.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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

