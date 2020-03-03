---
title: "eventMessageRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# eventMessageRequest resource type


Namespace: microsoft.graph




Inherits from [eventMessage](../resources/eventmessage.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List eventMessageRequests](../api/eventmessagerequest-list.md)|[eventMessageRequest](../resources/eventmessagerequest.md) collection|List properties and relationships of the [eventMessageRequest](../resources/eventmessagerequest.md) objects.|
|[Get eventMessageRequest](../api/eventmessagerequest-get.md)|[eventMessageRequest](../resources/eventmessagerequest.md)|Read properties and relationships of the [eventMessageRequest](../resources/eventmessagerequest.md) object.|
|[Create eventMessageRequest](../api/eventmessagerequest-create.md)|[eventMessageRequest](../resources/eventmessagerequest.md)|Create a new [eventMessageRequest](../resources/eventmessagerequest.md) object.|
|[Delete eventMessageRequest](../api/eventmessagerequest-delete.md)|None|Deletes a [eventMessageRequest](../resources/eventmessagerequest.md).|
|[Update eventMessageRequest](../api/eventmessagerequest-update.md)|[eventMessageRequest](../resources/eventmessagerequest.md)|Update the properties of a [eventMessageRequest](../resources/eventmessagerequest.md) object.|
|[accept](../api/eventmessagerequest-accept.md)|None||
|[decline](../api/eventmessagerequest-decline.md)|None||
|[tentativelyAccept](../api/eventmessagerequest-tentativelyaccept.md)|None||
|[List singleValueExtendedProperties](../api/eventmessagerequest-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/eventmessagerequest-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/eventmessagerequest-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/eventmessagerequest-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|
|[List attachments](../api/eventmessagerequest-list-attachments.md)|[attachment](../resources/attachment.md) collection|Get the attachments from the attachments navigation property.|
|[Add attachments](../api/eventmessagerequest-post-attachments.md)|[attachment](../resources/attachment.md)|Add attachments by posting to the attachments collection.|
|[List extensions](../api/eventmessagerequest-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Add extensions](../api/eventmessagerequest-post-extensions.md)|[extension](../resources/extension.md)|Add extensions by posting to the extensions collection.|
|[List mentions](../api/eventmessagerequest-list-mentions.md)|[mention](../resources/mention.md) collection|Get the mentions from the mentions navigation property.|
|[Add mentions](../api/eventmessagerequest-post-mentions.md)|[mention](../resources/mention.md)|Add mentions by posting to the mentions collection.|
|[Get event](../api/event-get.md)|[event](../resources/event.md)|Read properties and relationships of the [event](../resources/event.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowNewTimeProposals|Boolean||
|bccRecipients|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|body|[itemBody](../resources/itembody.md)| Inherited from [message](../resources/message.md)|
|bodyPreview|String| Inherited from [message](../resources/message.md)|
|categories|String collection| Inherited from [outlookItem](../resources/outlookitem.md)|
|ccRecipients|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|changeKey|String| Inherited from [outlookItem](../resources/outlookitem.md)|
|conversationId|String| Inherited from [message](../resources/message.md)|
|conversationIndex|Binary| Inherited from [message](../resources/message.md)|
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|endDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)| Inherited from [eventMessage](../resources/eventmessage.md)|
|flag|[followupFlag](../resources/followupflag.md)| Inherited from [message](../resources/message.md)|
|from|[recipient](../resources/recipient.md)| Inherited from [message](../resources/message.md)|
|hasAttachments|Boolean| Inherited from [message](../resources/message.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|importance|Enumeration| Inherited from [message](../resources/message.md). Possible values are: `low`, `normal`, `high`.|
|inferenceClassification|Enumeration| Inherited from [message](../resources/message.md). Possible values are: `focused`, `other`.|
|internetMessageHeaders|[internetMessageHeader](../resources/internetmessageheader.md) collection| Inherited from [message](../resources/message.md)|
|internetMessageId|String| Inherited from [message](../resources/message.md)|
|isAllDay|Boolean| Inherited from [eventMessage](../resources/eventmessage.md)|
|isDelegated|Boolean| Inherited from [eventMessage](../resources/eventmessage.md)|
|isDeliveryReceiptRequested|Boolean| Inherited from [message](../resources/message.md)|
|isDraft|Boolean| Inherited from [message](../resources/message.md)|
|isOutOfDate|Boolean| Inherited from [eventMessage](../resources/eventmessage.md)|
|isRead|Boolean| Inherited from [message](../resources/message.md)|
|isReadReceiptRequested|Boolean| Inherited from [message](../resources/message.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|location|[location](../resources/location.md)| Inherited from [eventMessage](../resources/eventmessage.md)|
|meetingMessageType|Enumeration| Inherited from [eventMessage](../resources/eventmessage.md). Possible values are: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTentativelyAccepted`, `meetingDeclined`.|
|mentionsPreview|[mentionsPreview](../resources/mentionspreview.md)| Inherited from [message](../resources/message.md)|
|parentFolderId|String| Inherited from [message](../resources/message.md)|
|previousEndDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|previousLocation|[location](../resources/location.md)||
|previousStartDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|receivedDateTime|DateTimeOffset| Inherited from [message](../resources/message.md)|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)| Inherited from [eventMessage](../resources/eventmessage.md)|
|replyTo|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|responseRequested|Boolean||
|sender|[recipient](../resources/recipient.md)| Inherited from [message](../resources/message.md)|
|sentDateTime|DateTimeOffset| Inherited from [message](../resources/message.md)|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)| Inherited from [eventMessage](../resources/eventmessage.md)|
|subject|String| Inherited from [message](../resources/message.md)|
|toRecipients|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|type|Enumeration| Inherited from [eventMessage](../resources/eventmessage.md). Possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.|
|uniqueBody|[itemBody](../resources/itembody.md)| Inherited from [message](../resources/message.md)|
|unsubscribeData|String collection| Inherited from [message](../resources/message.md)|
|unsubscribeEnabled|Boolean| Inherited from [message](../resources/message.md)|
|webLink|String| Inherited from [message](../resources/message.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|attachments|[attachment](../resources/attachment.md) collection| Inherited from [message](../resources/message.md)|
|event|[event](../resources/event.md)| Inherited from [eventMessage](../resources/eventmessage.md)|
|extensions|[extension](../resources/extension.md) collection| Inherited from [message](../resources/message.md)|
|mentions|[mention](../resources/mention.md) collection| Inherited from [message](../resources/message.md)|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection| Inherited from [message](../resources/message.md)|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection| Inherited from [message](../resources/message.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eventMessageRequest",
  "baseType": "microsoft.graph.eventMessage",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eventMessageRequest",
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
  "isDelegated": true,
  "previousLocation": {
    "@odata.type": "microsoft.graph.location"
  },
  "previousStartDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "previousEndDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "responseRequested": true,
  "allowNewTimeProposals": true
}
```

