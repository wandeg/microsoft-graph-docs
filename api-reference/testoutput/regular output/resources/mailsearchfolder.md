---
title: "mailSearchFolder resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mailSearchFolder resource type


Namespace: microsoft.graph




Inherits from [mailFolder](../resources/mailfolder.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List mailSearchFolders](../api/mailsearchfolder-list.md)|[mailSearchFolder](../resources/mailsearchfolder.md) collection|List properties and relationships of the [mailSearchFolder](../resources/mailsearchfolder.md) objects.|
|[Get mailSearchFolder](../api/mailsearchfolder-get.md)|[mailSearchFolder](../resources/mailsearchfolder.md)|Read properties and relationships of the [mailSearchFolder](../resources/mailsearchfolder.md) object.|
|[Create mailSearchFolder](../api/mailsearchfolder-create.md)|[mailSearchFolder](../resources/mailsearchfolder.md)|Create a new [mailSearchFolder](../resources/mailsearchfolder.md) object.|
|[Delete mailSearchFolder](../api/mailsearchfolder-delete.md)|None|Deletes a [mailSearchFolder](../resources/mailsearchfolder.md).|
|[Update mailSearchFolder](../api/mailsearchfolder-update.md)|[mailSearchFolder](../resources/mailsearchfolder.md)|Update the properties of a [mailSearchFolder](../resources/mailsearchfolder.md) object.|
|[copy](../api/mailsearchfolder-copy.md)|[mailFolder](../resources/mailfolder.md)||
|[move](../api/mailsearchfolder-move.md)|[mailFolder](../resources/mailfolder.md)||
|[List singleValueExtendedProperties](../api/mailsearchfolder-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/mailsearchfolder-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/mailsearchfolder-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/mailsearchfolder-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|
|[List messages](../api/mailsearchfolder-list-messages.md)|[message](../resources/message.md) collection|Get the messages from the messages navigation property.|
|[Add messages](../api/mailsearchfolder-post-messages.md)|[message](../resources/message.md)|Add messages by posting to the messages collection.|
|[List messageRules](../api/mailsearchfolder-list-messagerules.md)|[messageRule](../resources/messagerule.md) collection|Get the messageRules from the messageRules navigation property.|
|[Add messageRules](../api/mailsearchfolder-post-messagerules.md)|[messageRule](../resources/messagerule.md)|Add messageRules by posting to the messageRules collection.|
|[List childFolders](../api/mailsearchfolder-list-childfolders.md)|[mailFolder](../resources/mailfolder.md) collection|Get the mailFolders from the childFolders navigation property.|
|[Add childFolders](../api/mailsearchfolder-post-childfolders.md)|[mailFolder](../resources/mailfolder.md)|Add childFolders by posting to the childFolders collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|childFolderCount|Int32| Inherited from [mailFolder](../resources/mailfolder.md)|
|displayName|String| Inherited from [mailFolder](../resources/mailfolder.md)|
|filterQuery|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|includeNestedFolders|Boolean||
|isSupported|Boolean||
|parentFolderId|String| Inherited from [mailFolder](../resources/mailfolder.md)|
|sourceFolderIds|String collection||
|totalItemCount|Int32| Inherited from [mailFolder](../resources/mailfolder.md)|
|unreadItemCount|Int32| Inherited from [mailFolder](../resources/mailfolder.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|childFolders|[mailFolder](../resources/mailfolder.md) collection| Inherited from [mailFolder](../resources/mailfolder.md)|
|messageRules|[messageRule](../resources/messagerule.md) collection| Inherited from [mailFolder](../resources/mailfolder.md)|
|messages|[message](../resources/message.md) collection| Inherited from [mailFolder](../resources/mailfolder.md)|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection| Inherited from [mailFolder](../resources/mailfolder.md)|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection| Inherited from [mailFolder](../resources/mailfolder.md)|

## JSON Representation
Here is a JSON representation of the resource.
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
  "childFolderCount": 1024,
  "unreadItemCount": 1024,
  "totalItemCount": 1024,
  "isSupported": true,
  "includeNestedFolders": true,
  "sourceFolderIds": [
    "String"
  ],
  "filterQuery": "String"
}
```

