---
title: "message resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# message resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [outlookItem](../resources/outlookitem.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[createReply](../api/message-createreply.md)|[message](../resources/message.md)|**TODO: Add Description**|
|[createReplyAll](../api/message-createreplyall.md)|[message](../resources/message.md)|**TODO: Add Description**|
|[createForward](../api/message-createforward.md)|[message](../resources/message.md)|**TODO: Add Description**|
|[send](../api/message-send.md)|None|**TODO: Add Description**|
|[copy](../api/message-copy.md)|[message](../resources/message.md)|**TODO: Add Description**|
|[move](../api/message-move.md)|[message](../resources/message.md)|**TODO: Add Description**|
|[reply](../api/message-reply.md)|None|**TODO: Add Description**|
|[replyAll](../api/message-replyall.md)|None|**TODO: Add Description**|
|[forward](../api/message-forward.md)|None|**TODO: Add Description**|
|[unsubscribe](../api/message-unsubscribe.md)|None|**TODO: Add Description**|
|[delta](../api/message-delta.md)|[message](../resources/message.md) collection|**TODO: Add Description**|
|[List singleValueExtendedProperties](../api/message-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Create singleValueExtendedProperties](../api/message-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Create a new singleValueExtendedProperties object.|
|[Delete singleValueExtendedProperties](../api/message-delete-singlevalueextendedproperties.md)|None|Delete a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.|
|[Update singleValueExtendedProperties](../api/message-update-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Update the properties of a singleValueExtendedProperties object.|
|[Get singleValueLegacyExtendedProperty](../api/singlevaluelegacyextendedproperty-get.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Read the properties and relationships of a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.|
|[List multiValueExtendedProperties](../api/message-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Create multiValueExtendedProperties](../api/message-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Create a new multiValueExtendedProperties object.|
|[Delete multiValueExtendedProperties](../api/message-delete-multivalueextendedproperties.md)|None|Delete a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.|
|[Update multiValueExtendedProperties](../api/message-update-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Update the properties of a multiValueExtendedProperties object.|
|[Get multiValueLegacyExtendedProperty](../api/multivaluelegacyextendedproperty-get.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Read the properties and relationships of a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.|
|[List attachments](../api/message-list-attachments.md)|[attachment](../resources/attachment.md) collection|Get the attachments from the attachments navigation property.|
|[Create attachments](../api/message-post-attachments.md)|[attachment](../resources/attachment.md)|Create a new attachments object.|
|[Delete attachments](../api/message-delete-attachments.md)|None|Delete an [attachment](../resources/attachment.md) object.|
|[Update attachments](../api/message-update-attachments.md)|[attachment](../resources/attachment.md)|Update the properties of an attachments object.|
|[Get attachment](../api/attachment-get.md)|[attachment](../resources/attachment.md)|Read the properties and relationships of an [attachment](../resources/attachment.md) object.|
|[List extensions](../api/message-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Create extensions](../api/message-post-extensions.md)|[extension](../resources/extension.md)|Create a new extensions object.|
|[Delete extensions](../api/message-delete-extensions.md)|None|Delete an [extension](../resources/extension.md) object.|
|[Update extensions](../api/message-update-extensions.md)|[extension](../resources/extension.md)|Update the properties of an extensions object.|
|[Get extension](../api/extension-get.md)|[extension](../resources/extension.md)|Read the properties and relationships of an [extension](../resources/extension.md) object.|
|[List mentions](../api/message-list-mentions.md)|[mention](../resources/mention.md) collection|Get the mentions from the mentions navigation property.|
|[Create mentions](../api/message-post-mentions.md)|[mention](../resources/mention.md)|Create a new mentions object.|
|[Delete mentions](../api/message-delete-mentions.md)|None|Delete a [mention](../resources/mention.md) object.|
|[Update mentions](../api/message-update-mentions.md)|[mention](../resources/mention.md)|Update the properties of a mentions object.|
|[Get mention](../api/mention-get.md)|[mention](../resources/mention.md)|Read the properties and relationships of a [mention](../resources/mention.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bccRecipients|[recipient](../resources/recipient.md) collection|**TODO: Add Description**|
|body|[itemBody](../resources/itembody.md)|**TODO: Add Description**|
|bodyPreview|String|**TODO: Add Description**|
|categories|String collection|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|ccRecipients|[recipient](../resources/recipient.md) collection|**TODO: Add Description**|
|changeKey|String|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|conversationId|String|**TODO: Add Description**|
|conversationIndex|Binary|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|flag|[followupFlag](../resources/followupflag.md)|**TODO: Add Description**|
|from|[recipient](../resources/recipient.md)|**TODO: Add Description**|
|hasAttachments|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|importance|importance|**TODO: Add Description**. Possible values are: `low`, `normal`, `high`.|
|inferenceClassification|inferenceClassificationType|**TODO: Add Description**. Possible values are: `focused`, `other`.|
|internetMessageHeaders|[internetMessageHeader](../resources/internetmessageheader.md) collection|**TODO: Add Description**|
|internetMessageId|String|**TODO: Add Description**|
|isDeliveryReceiptRequested|Boolean|**TODO: Add Description**|
|isDraft|Boolean|**TODO: Add Description**|
|isRead|Boolean|**TODO: Add Description**|
|isReadReceiptRequested|Boolean|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|mentionsPreview|[mentionsPreview](../resources/mentionspreview.md)|**TODO: Add Description**|
|parentFolderId|String|**TODO: Add Description**|
|receivedDateTime|DateTimeOffset|**TODO: Add Description**|
|replyTo|[recipient](../resources/recipient.md) collection|**TODO: Add Description**|
|sender|[recipient](../resources/recipient.md)|**TODO: Add Description**|
|sentDateTime|DateTimeOffset|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|
|toRecipients|[recipient](../resources/recipient.md) collection|**TODO: Add Description**|
|uniqueBody|[itemBody](../resources/itembody.md)|**TODO: Add Description**|
|unsubscribeData|String collection|**TODO: Add Description**|
|unsubscribeEnabled|Boolean|**TODO: Add Description**|
|webLink|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|attachments|[attachment](../resources/attachment.md) collection|**TODO: Add Description**|
|extensions|[extension](../resources/extension.md) collection|**TODO: Add Description**|
|mentions|[mention](../resources/mention.md) collection|**TODO: Add Description**|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|**TODO: Add Description**|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.message",
  "baseType": "microsoft.graph.outlookItem",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.message",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "changeKey": "String",
  "categories": [
    "String"
  ],
  "receivedDateTime": "String (timestamp)",
  "sentDateTime": "String (timestamp)",
  "hasAttachments": "Boolean",
  "internetMessageId": "String",
  "internetMessageHeaders": [
    {
      "@odata.type": "microsoft.graph.internetMessageHeader"
    }
  ],
  "subject": "String",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "bodyPreview": "String",
  "importance": "String",
  "parentFolderId": "String",
  "sender": {
    "@odata.type": "microsoft.graph.recipient"
  },
  "from": {
    "@odata.type": "microsoft.graph.recipient"
  },
  "toRecipients": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "ccRecipients": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "bccRecipients": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "replyTo": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "conversationId": "String",
  "conversationIndex": "Binary",
  "uniqueBody": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "isDeliveryReceiptRequested": "Boolean",
  "isReadReceiptRequested": "Boolean",
  "isRead": "Boolean",
  "isDraft": "Boolean",
  "webLink": "String",
  "mentionsPreview": {
    "@odata.type": "microsoft.graph.mentionsPreview"
  },
  "inferenceClassification": "String",
  "unsubscribeData": [
    "String"
  ],
  "unsubscribeEnabled": "Boolean",
  "flag": {
    "@odata.type": "microsoft.graph.followupFlag"
  }
}
```

