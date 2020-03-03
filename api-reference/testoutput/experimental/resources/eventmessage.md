---
title: "eventMessage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# eventMessage resource type


Namespace: microsoft.graph




Inherits from [message](../resources/message.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List eventMessages](../api/eventmessage-list.md)|[eventMessage](../resources/eventmessage.md) collection|List properties and relationships of the [eventMessage](../resources/eventmessage.md) objects.|
|[Get eventMessage](../api/eventmessage-get.md)|[eventMessage](../resources/eventmessage.md)|Read properties and relationships of the [eventMessage](../resources/eventmessage.md) object.|
|[Create eventMessage](../api/eventmessage-create.md)|[eventMessage](../resources/eventmessage.md)|Create a new [eventMessage](../resources/eventmessage.md) object.|
|[Delete eventMessage](../api/eventmessage-delete.md)|None|Deletes a [eventMessage](../resources/eventmessage.md).|
|[Update eventMessage](../api/eventmessage-update.md)|[eventMessage](../resources/eventmessage.md)|Update the properties of a [eventMessage](../resources/eventmessage.md) object.|
|[createReply](../api/eventmessage-createreply.md)|[message](../resources/message.md)||
|[createReplyAll](../api/eventmessage-createreplyall.md)|[message](../resources/message.md)||
|[createForward](../api/eventmessage-createforward.md)|[message](../resources/message.md)||
|[send](../api/eventmessage-send.md)|None||
|[copy](../api/eventmessage-copy.md)|[message](../resources/message.md)||
|[move](../api/eventmessage-move.md)|[message](../resources/message.md)||
|[reply](../api/eventmessage-reply.md)|None||
|[replyAll](../api/eventmessage-replyall.md)|None||
|[forward](../api/eventmessage-forward.md)|None||
|[unsubscribe](../api/eventmessage-unsubscribe.md)|None||
|[List singleValueExtendedProperties](../api/eventmessage-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/eventmessage-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/eventmessage-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/eventmessage-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|
|[List attachments](../api/eventmessage-list-attachments.md)|[attachment](../resources/attachment.md) collection|Get the attachments from the attachments navigation property.|
|[Add attachments](../api/eventmessage-post-attachments.md)|[attachment](../resources/attachment.md)|Add attachments by posting to the attachments collection.|
|[List extensions](../api/eventmessage-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Add extensions](../api/eventmessage-post-extensions.md)|[extension](../resources/extension.md)|Add extensions by posting to the extensions collection.|
|[List mentions](../api/eventmessage-list-mentions.md)|[mention](../resources/mention.md) collection|Get the mentions from the mentions navigation property.|
|[Add mentions](../api/eventmessage-post-mentions.md)|[mention](../resources/mention.md)|Add mentions by posting to the mentions collection.|
|[Get event](../api/event-get.md)|[event](../resources/event.md)|Read properties and relationships of the [event](../resources/event.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bccRecipients|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|body|[itemBody](../resources/itembody.md)| Inherited from [message](../resources/message.md)|
|bodyPreview|String| Inherited from [message](../resources/message.md)|
|categories|String collection| Inherited from [outlookItem](../resources/outlookitem.md)|
|ccRecipients|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|changeKey|String| Inherited from [outlookItem](../resources/outlookitem.md)|
|conversationId|String| Inherited from [message](../resources/message.md)|
|conversationIndex|Binary| Inherited from [message](../resources/message.md)|
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|endDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|flag|[followupFlag](../resources/followupflag.md)| Inherited from [message](../resources/message.md)|
|from|[recipient](../resources/recipient.md)| Inherited from [message](../resources/message.md)|
|hasAttachments|Boolean| Inherited from [message](../resources/message.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|importance|Enumeration| Inherited from [message](../resources/message.md). Possible values are: `low`, `normal`, `high`.|
|inferenceClassification|Enumeration| Inherited from [message](../resources/message.md). Possible values are: `focused`, `other`.|
|internetMessageHeaders|[internetMessageHeader](../resources/internetmessageheader.md) collection| Inherited from [message](../resources/message.md)|
|internetMessageId|String| Inherited from [message](../resources/message.md)|
|isAllDay|Boolean||
|isDelegated|Boolean||
|isDeliveryReceiptRequested|Boolean| Inherited from [message](../resources/message.md)|
|isDraft|Boolean| Inherited from [message](../resources/message.md)|
|isOutOfDate|Boolean||
|isRead|Boolean| Inherited from [message](../resources/message.md)|
|isReadReceiptRequested|Boolean| Inherited from [message](../resources/message.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|location|[location](../resources/location.md)||
|meetingMessageType|Enumeration|. Possible values are: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTentativelyAccepted`, `meetingDeclined`.|
|mentionsPreview|[mentionsPreview](../resources/mentionspreview.md)| Inherited from [message](../resources/message.md)|
|parentFolderId|String| Inherited from [message](../resources/message.md)|
|receivedDateTime|DateTimeOffset| Inherited from [message](../resources/message.md)|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)||
|replyTo|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|sender|[recipient](../resources/recipient.md)| Inherited from [message](../resources/message.md)|
|sentDateTime|DateTimeOffset| Inherited from [message](../resources/message.md)|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|subject|String| Inherited from [message](../resources/message.md)|
|toRecipients|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|type|Enumeration|. Possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.|
|uniqueBody|[itemBody](../resources/itembody.md)| Inherited from [message](../resources/message.md)|
|unsubscribeData|String collection| Inherited from [message](../resources/message.md)|
|unsubscribeEnabled|Boolean| Inherited from [message](../resources/message.md)|
|webLink|String| Inherited from [message](../resources/message.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|attachments|[attachment](../resources/attachment.md) collection| Inherited from [message](../resources/message.md)|
|event|[event](../resources/event.md)||
|extensions|[extension](../resources/extension.md) collection| Inherited from [message](../resources/message.md)|
|mentions|[mention](../resources/mention.md) collection| Inherited from [message](../resources/message.md)|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection| Inherited from [message](../resources/message.md)|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection| Inherited from [message](../resources/message.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eventMessage",
  "baseType": "microsoft.graph.message",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eventMessage",
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
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "dueDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "startDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "flagStatus": "String"
  },
  "meetingMessageType": "String",
  "startDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "endDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "location": {
    "@odata.type": "microsoft.graph.location"
  },
  "type": "String",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "isOutOfDate": true,
  "isAllDay": true,
  "isDelegated": true
}
```

