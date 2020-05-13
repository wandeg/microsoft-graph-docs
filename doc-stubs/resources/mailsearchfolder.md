---
title: "mailSearchFolder resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mailSearchFolder resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [mailFolder](../resources/mailfolder.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[copy](../api/mailsearchfolder-copy.md)|[mailFolder](../resources/mailfolder.md)|**TODO: Add Description**|
|[move](../api/mailsearchfolder-move.md)|[mailFolder](../resources/mailfolder.md)|**TODO: Add Description**|
|[List singleValueExtendedProperties](../api/mailsearchfolder-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Create singleValueExtendedProperties](../api/mailsearchfolder-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Create a new singleValueExtendedProperties object.|
|[Delete singleValueExtendedProperties](../api/mailsearchfolder-delete-singlevalueextendedproperties.md)|None|Delete a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.|
|[Update singleValueExtendedProperties](../api/mailsearchfolder-update-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Update the properties of a singleValueExtendedProperties object.|
|[Get singleValueExtendedProperties](../api/mailsearchfolder-get-singlevaluelegacyextendedproperty.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Read the properties and relationships of a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.|
|[List multiValueExtendedProperties](../api/mailsearchfolder-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Create multiValueExtendedProperties](../api/mailsearchfolder-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Create a new multiValueExtendedProperties object.|
|[Delete multiValueExtendedProperties](../api/mailsearchfolder-delete-multivalueextendedproperties.md)|None|Delete a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.|
|[Update multiValueExtendedProperties](../api/mailsearchfolder-update-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Update the properties of a multiValueExtendedProperties object.|
|[Get multiValueExtendedProperties](../api/mailsearchfolder-get-multivaluelegacyextendedproperty.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Read the properties and relationships of a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.|
|[List messages](../api/mailsearchfolder-list-messages.md)|[message](../resources/message.md) collection|Get the messages from the messages navigation property.|
|[Create messages](../api/mailsearchfolder-post-messages.md)|[message](../resources/message.md)|Create a new messages object.|
|[Delete messages](../api/mailsearchfolder-delete-messages.md)|None|Delete a [message](../resources/message.md) object.|
|[Update messages](../api/mailsearchfolder-update-messages.md)|[message](../resources/message.md)|Update the properties of a messages object.|
|[Get messages](../api/mailsearchfolder-get-message.md)|[message](../resources/message.md)|Read the properties and relationships of a [message](../resources/message.md) object.|
|[List messageRules](../api/mailsearchfolder-list-messagerules.md)|[messageRule](../resources/messagerule.md) collection|Get the messageRules from the messageRules navigation property.|
|[Create messageRules](../api/mailsearchfolder-post-messagerules.md)|[messageRule](../resources/messagerule.md)|Create a new messageRules object.|
|[Delete messageRules](../api/mailsearchfolder-delete-messagerules.md)|None|Delete a [messageRule](../resources/messagerule.md) object.|
|[Update messageRules](../api/mailsearchfolder-update-messagerules.md)|[messageRule](../resources/messagerule.md)|Update the properties of a messageRules object.|
|[Get messageRules](../api/mailsearchfolder-get-messagerule.md)|[messageRule](../resources/messagerule.md)|Read the properties and relationships of a [messageRule](../resources/messagerule.md) object.|
|[List childFolders](../api/mailsearchfolder-list-childfolders.md)|[mailFolder](../resources/mailfolder.md) collection|Get the mailFolders from the childFolders navigation property.|
|[Create childFolders](../api/mailsearchfolder-post-childfolders.md)|[mailFolder](../resources/mailfolder.md)|Create a new childFolders object.|
|[Delete childFolders](../api/mailsearchfolder-delete-childfolders.md)|None|Delete a [mailFolder](../resources/mailfolder.md) object.|
|[Update childFolders](../api/mailsearchfolder-update-childfolders.md)|[mailFolder](../resources/mailfolder.md)|Update the properties of a childFolders object.|
|[Get childFolders](../api/mailsearchfolder-get-mailfolder.md)|[mailFolder](../resources/mailfolder.md)|Read the properties and relationships of a [mailFolder](../resources/mailfolder.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|childFolderCount|Int32|**TODO: Add Description** Inherited from [mailFolder](../resources/mailfolder.md)|
|displayName|String|**TODO: Add Description** Inherited from [mailFolder](../resources/mailfolder.md)|
|filterQuery|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|includeNestedFolders|Boolean|**TODO: Add Description**|
|isSupported|Boolean|**TODO: Add Description**|
|parentFolderId|String|**TODO: Add Description** Inherited from [mailFolder](../resources/mailfolder.md)|
|sourceFolderIds|String collection|**TODO: Add Description**|
|totalItemCount|Int32|**TODO: Add Description** Inherited from [mailFolder](../resources/mailfolder.md)|
|unreadItemCount|Int32|**TODO: Add Description** Inherited from [mailFolder](../resources/mailfolder.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|childFolders|[mailFolder](../resources/mailfolder.md) collection|**TODO: Add Description** Inherited from [mailFolder](../resources/mailfolder.md)|
|messageRules|[messageRule](../resources/messagerule.md) collection|**TODO: Add Description** Inherited from [mailFolder](../resources/mailfolder.md)|
|messages|[message](../resources/message.md) collection|**TODO: Add Description** Inherited from [mailFolder](../resources/mailfolder.md)|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|**TODO: Add Description** Inherited from [mailFolder](../resources/mailfolder.md)|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|**TODO: Add Description** Inherited from [mailFolder](../resources/mailfolder.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "baseType": "microsoft.graph.mailFolder",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mailSearchFolder",
  "id": "String (identifier)",
  "displayName": "String",
  "parentFolderId": "String",
  "childFolderCount": "Integer",
  "unreadItemCount": "Integer",
  "totalItemCount": "Integer",
  "isSupported": "Boolean",
  "includeNestedFolders": "Boolean",
  "sourceFolderIds": [
    "String"
  ],
  "filterQuery": "String"
}
```

