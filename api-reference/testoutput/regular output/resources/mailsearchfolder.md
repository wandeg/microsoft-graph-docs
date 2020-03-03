---
title: "mailSearchFolder resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# mailSearchFolder resource type




Inherits from [mailFolder](../resources/mailFolder.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List mailSearchFolders](../api/mailsearchfolder-list.md)|[mailSearchFolder](../resources/mailSearchFolder.md) collection|List properties and relationships of the [mailSearchFolder](../resources/mailsearchfolder.md) objects.|
|[Get mailSearchFolder](../api/mailsearchfolder-get.md)|[mailSearchFolder](../resources/mailSearchFolder.md)|Read properties and relationships of the [mailSearchFolder](../resources/mailsearchfolder.md) object.|
|[Create mailSearchFolder](../api/mailsearchfolder-create.md)|[mailSearchFolder](../resources/mailSearchFolder.md)|Create a new [mailSearchFolder](../resources/mailsearchfolder.md) object.|
|[Delete mailSearchFolder](../api/mailsearchfolder-delete.md)|None|Deletes a [mailSearchFolder](../resources/mailsearchfolder.md).|
|[Update mailSearchFolder](../api/mailsearchfolder-update.md)|[mailSearchFolder](../resources/mailSearchFolder.md)|Update the properties of a [mailSearchFolder](../resources/mailsearchfolder.md) object.|
|[copy](../api/mailsearchfolder-copy.md)|[mailFolder](../resources/mailFolder.md)||
|[move](../api/mailsearchfolder-move.md)|[mailFolder](../resources/mailFolder.md)||
|[List singleValueExtendedProperties](../api/mailsearchfolder-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/mailsearchfolder-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/mailsearchfolder-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/mailsearchfolder-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|
|[List messages](../api/mailsearchfolder-list-messages.md)|[message](../resources/message.md) collection|Get the messages from the messages navigation property.|
|[Add messages](../api/mailsearchfolder-post-messages.md)|[message](../resources/message.md)|Add messages by posting to the messages collection.|
|[List messageRules](../api/mailsearchfolder-list-messagerules.md)|[messageRule](../resources/messageRule.md) collection|Get the messageRules from the messageRules navigation property.|
|[Add messageRules](../api/mailsearchfolder-post-messagerules.md)|[messageRule](../resources/messageRule.md)|Add messageRules by posting to the messageRules collection.|
|[List childFolders](../api/mailsearchfolder-list-childfolders.md)|[mailFolder](../resources/mailFolder.md) collection|Get the mailFolders from the childFolders navigation property.|
|[Add childFolders](../api/mailsearchfolder-post-childfolders.md)|[mailFolder](../resources/mailFolder.md)|Add childFolders by posting to the childFolders collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|childFolderCount|Int32| Inherited from [mailFolder](../resources/mailFolder.md)|
|displayName|String| Inherited from [mailFolder](../resources/mailFolder.md)|
|filterQuery|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|includeNestedFolders|Boolean||
|isSupported|Boolean||
|parentFolderId|String| Inherited from [mailFolder](../resources/mailFolder.md)|
|sourceFolderIds|String collection||
|totalItemCount|Int32| Inherited from [mailFolder](../resources/mailFolder.md)|
|unreadItemCount|Int32| Inherited from [mailFolder](../resources/mailFolder.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|childFolders|[mailFolder](../resources/mailFolder.md) collection| Inherited from [mailFolder](../resources/mailFolder.md)|
|messageRules|[messageRule](../resources/messageRule.md) collection| Inherited from [mailFolder](../resources/mailFolder.md)|
|messages|[message](../resources/message.md) collection| Inherited from [mailFolder](../resources/mailFolder.md)|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) collection| Inherited from [mailFolder](../resources/mailFolder.md)|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) collection| Inherited from [mailFolder](../resources/mailFolder.md)|

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

