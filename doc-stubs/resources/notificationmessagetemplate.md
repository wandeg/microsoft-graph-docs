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
|[sendTestMessage](../api/notificationmessagetemplate-sendtestmessage.md)|None|**TODO: Add Description**|
|[List localizedNotificationMessages](../api/notificationmessagetemplate-list-localizednotificationmessages.md)|[localizedNotificationMessage](../resources/localizednotificationmessage.md) collection|Get the localizedNotificationMessages from the localizedNotificationMessages navigation property.|
|[Create localizedNotificationMessages](../api/notificationmessagetemplate-post-localizednotificationmessages.md)|[localizedNotificationMessage](../resources/localizednotificationmessage.md)|Create a new localizedNotificationMessages object.|
|[Delete localizedNotificationMessages](../api/notificationmessagetemplate-delete-localizednotificationmessages.md)|None|Delete a [localizedNotificationMessage](../resources/localizednotificationmessage.md) object.|
|[Update localizedNotificationMessages](../api/notificationmessagetemplate-update-localizednotificationmessages.md)|[localizedNotificationMessage](../resources/localizednotificationmessage.md)|Update the properties of a localizedNotificationMessages object.|
|[Get localizedNotificationMessage](../api/localizednotificationmessage-get.md)|[localizedNotificationMessage](../resources/localizednotificationmessage.md)|Read the properties and relationships of a [localizedNotificationMessage](../resources/localizednotificationmessage.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|brandingOptions|notificationTemplateBrandingOptions|**TODO: Add Description**. Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.|
|defaultLocale|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|localizedNotificationMessages|[localizedNotificationMessage](../resources/localizednotificationmessage.md) collection|**TODO: Add Description**|

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
  "brandingOptions": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```

