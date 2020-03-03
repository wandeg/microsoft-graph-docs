---
title: "eventMessageResponse resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# eventMessageResponse resource type




Inherits from [eventMessage](../resources/eventMessage.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List eventMessageResponses](../api/eventmessageresponse-list.md)|[eventMessageResponse](../resources/eventMessageResponse.md) collection|List properties and relationships of the [eventMessageResponse](../resources/eventmessageresponse.md) objects.|
|[Get eventMessageResponse](../api/eventmessageresponse-get.md)|[eventMessageResponse](../resources/eventMessageResponse.md)|Read properties and relationships of the [eventMessageResponse](../resources/eventmessageresponse.md) object.|
|[Create eventMessageResponse](../api/eventmessageresponse-create.md)|[eventMessageResponse](../resources/eventMessageResponse.md)|Create a new [eventMessageResponse](../resources/eventmessageresponse.md) object.|
|[Delete eventMessageResponse](../api/eventmessageresponse-delete.md)|None|Deletes a [eventMessageResponse](../resources/eventmessageresponse.md).|
|[Update eventMessageResponse](../api/eventmessageresponse-update.md)|[eventMessageResponse](../resources/eventMessageResponse.md)|Update the properties of a [eventMessageResponse](../resources/eventmessageresponse.md) object.|
|[List singleValueExtendedProperties](../api/eventmessageresponse-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/eventmessageresponse-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/eventmessageresponse-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/eventmessageresponse-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|
|[List attachments](../api/eventmessageresponse-list-attachments.md)|[attachment](../resources/attachment.md) collection|Get the attachments from the attachments navigation property.|
|[Add attachments](../api/eventmessageresponse-post-attachments.md)|[attachment](../resources/attachment.md)|Add attachments by posting to the attachments collection.|
|[List extensions](../api/eventmessageresponse-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Add extensions](../api/eventmessageresponse-post-extensions.md)|[extension](../resources/extension.md)|Add extensions by posting to the extensions collection.|
|[List mentions](../api/eventmessageresponse-list-mentions.md)|[mention](../resources/mention.md) collection|Get the mentions from the mentions navigation property.|
|[Add mentions](../api/eventmessageresponse-post-mentions.md)|[mention](../resources/mention.md)|Add mentions by posting to the mentions collection.|
|[Get event](../api/event-get.md)|[event](../resources/event.md)|Read properties and relationships of the [event](../resources/event.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bccRecipients|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|body|[itemBody](../resources/itemBody.md)| Inherited from [message](../resources/message.md)|
|bodyPreview|String| Inherited from [message](../resources/message.md)|
|categories|String collection| Inherited from [outlookItem](../resources/outlookItem.md)|
|ccRecipients|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|changeKey|String| Inherited from [outlookItem](../resources/outlookItem.md)|
|conversationId|String| Inherited from [message](../resources/message.md)|
|conversationIndex|Binary| Inherited from [message](../resources/message.md)|
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookItem.md)|
|endDateTime|[dateTimeTimeZone](../resources/dateTimeTimeZone.md)| Inherited from [eventMessage](../resources/eventMessage.md)|
|flag|[followupFlag](../resources/followupFlag.md)| Inherited from [message](../resources/message.md)|
|from|[recipient](../resources/recipient.md)| Inherited from [message](../resources/message.md)|
|hasAttachments|Boolean| Inherited from [message](../resources/message.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|importance|Enumeration| Inherited from [message](../resources/message.md). Possible values are: `low`, `normal`, `high`.|
|inferenceClassification|Enumeration| Inherited from [message](../resources/message.md). Possible values are: `focused`, `other`.|
|internetMessageHeaders|[internetMessageHeader](../resources/internetMessageHeader.md) collection| Inherited from [message](../resources/message.md)|
|internetMessageId|String| Inherited from [message](../resources/message.md)|
|isAllDay|Boolean| Inherited from [eventMessage](../resources/eventMessage.md)|
|isDelegated|Boolean| Inherited from [eventMessage](../resources/eventMessage.md)|
|isDeliveryReceiptRequested|Boolean| Inherited from [message](../resources/message.md)|
|isDraft|Boolean| Inherited from [message](../resources/message.md)|
|isOutOfDate|Boolean| Inherited from [eventMessage](../resources/eventMessage.md)|
|isRead|Boolean| Inherited from [message](../resources/message.md)|
|isReadReceiptRequested|Boolean| Inherited from [message](../resources/message.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookItem.md)|
|location|[location](../resources/location.md)| Inherited from [eventMessage](../resources/eventMessage.md)|
|meetingMessageType|Enumeration| Inherited from [eventMessage](../resources/eventMessage.md). Possible values are: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTentativelyAccepted`, `meetingDeclined`.|
|mentionsPreview|[mentionsPreview](../resources/mentionsPreview.md)| Inherited from [message](../resources/message.md)|
|parentFolderId|String| Inherited from [message](../resources/message.md)|
|proposedNewTime|[timeSlot](../resources/timeSlot.md)||
|receivedDateTime|DateTimeOffset| Inherited from [message](../resources/message.md)|
|recurrence|[patternedRecurrence](../resources/patternedRecurrence.md)| Inherited from [eventMessage](../resources/eventMessage.md)|
|replyTo|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|responseType|Enumeration|. Possible values are: `none`, `organizer`, `tentativelyAccepted`, `accepted`, `declined`, `notResponded`.|
|sender|[recipient](../resources/recipient.md)| Inherited from [message](../resources/message.md)|
|sentDateTime|DateTimeOffset| Inherited from [message](../resources/message.md)|
|startDateTime|[dateTimeTimeZone](../resources/dateTimeTimeZone.md)| Inherited from [eventMessage](../resources/eventMessage.md)|
|subject|String| Inherited from [message](../resources/message.md)|
|toRecipients|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|type|Enumeration| Inherited from [eventMessage](../resources/eventMessage.md). Possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.|
|uniqueBody|[itemBody](../resources/itemBody.md)| Inherited from [message](../resources/message.md)|
|unsubscribeData|String collection| Inherited from [message](../resources/message.md)|
|unsubscribeEnabled|Boolean| Inherited from [message](../resources/message.md)|
|webLink|String| Inherited from [message](../resources/message.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|attachments|[attachment](../resources/attachment.md) collection| Inherited from [message](../resources/message.md)|
|event|[event](../resources/event.md)| Inherited from [eventMessage](../resources/eventMessage.md)|
|extensions|[extension](../resources/extension.md) collection| Inherited from [message](../resources/message.md)|
|mentions|[mention](../resources/mention.md) collection| Inherited from [message](../resources/message.md)|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multiValueLegacyExtendedProperty.md) collection| Inherited from [message](../resources/message.md)|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singleValueLegacyExtendedProperty.md) collection| Inherited from [message](../resources/message.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.eventMessageResponse",
  "baseType": "microsoft.graph.eventMessage",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.eventMessageResponse",
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
  "proposedNewTime": {
    "@odata.type": "microsoft.graph.timeSlot"
  },
  "responseType": "String"
}
```

