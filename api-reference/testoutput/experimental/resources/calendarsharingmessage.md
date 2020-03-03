---
title: "calendarSharingMessage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# calendarSharingMessage resource type


Namespace: microsoft.graph




Inherits from [message](../resources/message.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List calendarSharingMessages](../api/calendarsharingmessage-list.md)|[calendarSharingMessage](../resources/calendarsharingmessage.md) collection|List properties and relationships of the [calendarSharingMessage](../resources/calendarsharingmessage.md) objects.|
|[Get calendarSharingMessage](../api/calendarsharingmessage-get.md)|[calendarSharingMessage](../resources/calendarsharingmessage.md)|Read properties and relationships of the [calendarSharingMessage](../resources/calendarsharingmessage.md) object.|
|[Create calendarSharingMessage](../api/calendarsharingmessage-create.md)|[calendarSharingMessage](../resources/calendarsharingmessage.md)|Create a new [calendarSharingMessage](../resources/calendarsharingmessage.md) object.|
|[Delete calendarSharingMessage](../api/calendarsharingmessage-delete.md)|None|Deletes a [calendarSharingMessage](../resources/calendarsharingmessage.md).|
|[Update calendarSharingMessage](../api/calendarsharingmessage-update.md)|[calendarSharingMessage](../resources/calendarsharingmessage.md)|Update the properties of a [calendarSharingMessage](../resources/calendarsharingmessage.md) object.|
|[createReply](../api/calendarsharingmessage-createreply.md)|[message](../resources/message.md)||
|[createReplyAll](../api/calendarsharingmessage-createreplyall.md)|[message](../resources/message.md)||
|[createForward](../api/calendarsharingmessage-createforward.md)|[message](../resources/message.md)||
|[send](../api/calendarsharingmessage-send.md)|None||
|[copy](../api/calendarsharingmessage-copy.md)|[message](../resources/message.md)||
|[move](../api/calendarsharingmessage-move.md)|[message](../resources/message.md)||
|[reply](../api/calendarsharingmessage-reply.md)|None||
|[replyAll](../api/calendarsharingmessage-replyall.md)|None||
|[forward](../api/calendarsharingmessage-forward.md)|None||
|[unsubscribe](../api/calendarsharingmessage-unsubscribe.md)|None||
|[accept](../api/calendarsharingmessage-accept.md)|[calendar](../resources/calendar.md)||
|[List singleValueExtendedProperties](../api/calendarsharingmessage-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/calendarsharingmessage-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/calendarsharingmessage-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/calendarsharingmessage-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|
|[List attachments](../api/calendarsharingmessage-list-attachments.md)|[attachment](../resources/attachment.md) collection|Get the attachments from the attachments navigation property.|
|[Add attachments](../api/calendarsharingmessage-post-attachments.md)|[attachment](../resources/attachment.md)|Add attachments by posting to the attachments collection.|
|[List extensions](../api/calendarsharingmessage-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Add extensions](../api/calendarsharingmessage-post-extensions.md)|[extension](../resources/extension.md)|Add extensions by posting to the extensions collection.|
|[List mentions](../api/calendarsharingmessage-list-mentions.md)|[mention](../resources/mention.md) collection|Get the mentions from the mentions navigation property.|
|[Add mentions](../api/calendarsharingmessage-post-mentions.md)|[mention](../resources/mention.md)|Add mentions by posting to the mentions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bccRecipients|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|body|[itemBody](../resources/itembody.md)| Inherited from [message](../resources/message.md)|
|bodyPreview|String| Inherited from [message](../resources/message.md)|
|canAccept|Boolean||
|categories|String collection| Inherited from [outlookItem](../resources/outlookitem.md)|
|ccRecipients|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|changeKey|String| Inherited from [outlookItem](../resources/outlookitem.md)|
|conversationId|String| Inherited from [message](../resources/message.md)|
|conversationIndex|Binary| Inherited from [message](../resources/message.md)|
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|flag|[followupFlag](../resources/followupflag.md)| Inherited from [message](../resources/message.md)|
|from|[recipient](../resources/recipient.md)| Inherited from [message](../resources/message.md)|
|hasAttachments|Boolean| Inherited from [message](../resources/message.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|importance|Enumeration| Inherited from [message](../resources/message.md). Possible values are: `low`, `normal`, `high`.|
|inferenceClassification|Enumeration| Inherited from [message](../resources/message.md). Possible values are: `focused`, `other`.|
|internetMessageHeaders|[internetMessageHeader](../resources/internetmessageheader.md) collection| Inherited from [message](../resources/message.md)|
|internetMessageId|String| Inherited from [message](../resources/message.md)|
|isDeliveryReceiptRequested|Boolean| Inherited from [message](../resources/message.md)|
|isDraft|Boolean| Inherited from [message](../resources/message.md)|
|isRead|Boolean| Inherited from [message](../resources/message.md)|
|isReadReceiptRequested|Boolean| Inherited from [message](../resources/message.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|mentionsPreview|[mentionsPreview](../resources/mentionspreview.md)| Inherited from [message](../resources/message.md)|
|parentFolderId|String| Inherited from [message](../resources/message.md)|
|receivedDateTime|DateTimeOffset| Inherited from [message](../resources/message.md)|
|replyTo|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|sender|[recipient](../resources/recipient.md)| Inherited from [message](../resources/message.md)|
|sentDateTime|DateTimeOffset| Inherited from [message](../resources/message.md)|
|sharingMessageAction|[calendarSharingMessageAction](../resources/calendarsharingmessageaction.md)||
|sharingMessageActions|[calendarSharingMessageAction](../resources/calendarsharingmessageaction.md) collection||
|subject|String| Inherited from [message](../resources/message.md)|
|suggestedCalendarName|String||
|toRecipients|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|uniqueBody|[itemBody](../resources/itembody.md)| Inherited from [message](../resources/message.md)|
|unsubscribeData|String collection| Inherited from [message](../resources/message.md)|
|unsubscribeEnabled|Boolean| Inherited from [message](../resources/message.md)|
|webLink|String| Inherited from [message](../resources/message.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|attachments|[attachment](../resources/attachment.md) collection| Inherited from [message](../resources/message.md)|
|extensions|[extension](../resources/extension.md) collection| Inherited from [message](../resources/message.md)|
|mentions|[mention](../resources/mention.md) collection| Inherited from [message](../resources/message.md)|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection| Inherited from [message](../resources/message.md)|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection| Inherited from [message](../resources/message.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendarSharingMessage",
  "baseType": "microsoft.graph.message",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.calendarSharingMessage",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "changeKey": "String",
  "categories": [
    "String"
  ],
  "receivedDateTime": "String (timestamp)",
  "sentDateTime": "String (timestamp)",
  "hasAttachments": true,
  "internetMessageId": "String",
  "internetMessageHeaders": [
    {
      "@odata.type": "microsoft.graph.internetMessageHeader",
      "value": "String"
    }
  ],
  "subject": "String",
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "String"
  },
  "bodyPreview": "String",
  "importance": "String",
  "parentFolderId": "String",
  "sender": {
    "@odata.type": "microsoft.graph.recipient",
    "emailAddress": {
      "@odata.type": "microsoft.graph.emailAddress"
    }
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
  "conversationIndex": "binary",
  "uniqueBody": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "isDeliveryReceiptRequested": true,
  "isReadReceiptRequested": true,
  "isRead": true,
  "isDraft": true,
  "webLink": "String",
  "mentionsPreview": {
    "@odata.type": "microsoft.graph.mentionsPreview",
    "isMentioned": true
  },
  "inferenceClassification": "String",
  "unsubscribeData": [
    "String"
  ],
  "unsubscribeEnabled": true,
  "flag": {
    "@odata.type": "microsoft.graph.followupFlag",
    "completedDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone",
      "dateTime": "String",
      "timeZone": "String"
    },
    "dueDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "startDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "flagStatus": "String"
  },
  "canAccept": true,
  "suggestedCalendarName": "String",
  "sharingMessageAction": {
    "@odata.type": "microsoft.graph.calendarSharingMessageAction",
    "importance": "String",
    "actionType": "String",
    "action": "String"
  },
  "sharingMessageActions": [
    {
      "@odata.type": "microsoft.graph.calendarSharingMessageAction"
    }
  ]
}
```

