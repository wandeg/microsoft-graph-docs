---
title: "eventMessageResponse resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# eventMessageResponse resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [eventMessage](../resources/eventmessage.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List singleValueExtendedProperties](../api/eventmessageresponse-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Create singleValueExtendedProperties](../api/eventmessageresponse-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Create a new singleValueExtendedProperties object.|
|[Delete singleValueExtendedProperties](../api/eventmessageresponse-delete-singlevalueextendedproperties.md)|None|Delete a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.|
|[Update singleValueExtendedProperties](../api/eventmessageresponse-update-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Update the properties of a singleValueExtendedProperties object.|
|[Get singleValueExtendedProperties](../api/eventmessageresponse-get-singlevaluelegacyextendedproperty.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Read the properties and relationships of a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.|
|[List multiValueExtendedProperties](../api/eventmessageresponse-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Create multiValueExtendedProperties](../api/eventmessageresponse-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Create a new multiValueExtendedProperties object.|
|[Delete multiValueExtendedProperties](../api/eventmessageresponse-delete-multivalueextendedproperties.md)|None|Delete a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.|
|[Update multiValueExtendedProperties](../api/eventmessageresponse-update-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Update the properties of a multiValueExtendedProperties object.|
|[Get multiValueExtendedProperties](../api/eventmessageresponse-get-multivaluelegacyextendedproperty.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Read the properties and relationships of a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.|
|[List attachments](../api/eventmessageresponse-list-attachments.md)|[attachment](../resources/attachment.md) collection|Get the attachments from the attachments navigation property.|
|[Create attachments](../api/eventmessageresponse-post-attachments.md)|[attachment](../resources/attachment.md)|Create a new attachments object.|
|[Delete attachments](../api/eventmessageresponse-delete-attachments.md)|None|Delete an [attachment](../resources/attachment.md) object.|
|[Update attachments](../api/eventmessageresponse-update-attachments.md)|[attachment](../resources/attachment.md)|Update the properties of an attachments object.|
|[Get attachments](../api/eventmessageresponse-get-attachment.md)|[attachment](../resources/attachment.md)|Read the properties and relationships of an [attachment](../resources/attachment.md) object.|
|[List extensions](../api/eventmessageresponse-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Create extensions](../api/eventmessageresponse-post-extensions.md)|[extension](../resources/extension.md)|Create a new extensions object.|
|[Delete extensions](../api/eventmessageresponse-delete-extensions.md)|None|Delete an [extension](../resources/extension.md) object.|
|[Update extensions](../api/eventmessageresponse-update-extensions.md)|[extension](../resources/extension.md)|Update the properties of an extensions object.|
|[Get extensions](../api/eventmessageresponse-get-extension.md)|[extension](../resources/extension.md)|Read the properties and relationships of an [extension](../resources/extension.md) object.|
|[List event](../api/eventmessageresponse-list-event.md)|[event](../resources/event.md) collection|Get the events from the event navigation property.|
|[Create event](../api/eventmessageresponse-post-event.md)|[event](../resources/event.md)|Create a new event object.|
|[Delete event](../api/eventmessageresponse-delete-event.md)|None|Delete an [event](../resources/event.md) object.|
|[Update event](../api/eventmessageresponse-update-event.md)|[event](../resources/event.md)|Update the properties of an event object.|
|[Get event](../api/eventmessageresponse-get-event.md)|[event](../resources/event.md)|Read the properties and relationships of an [event](../resources/event.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bccRecipients|[recipient](../resources/recipient.md) collection|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|body|[itemBody](../resources/itembody.md)|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|bodyPreview|String|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|categories|String collection|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|ccRecipients|[recipient](../resources/recipient.md) collection|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|changeKey|String|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|conversationId|String|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|conversationIndex|Binary|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|endDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description** Inherited from [eventMessage](../resources/eventmessage.md)|
|flag|[followupFlag](../resources/followupflag.md)|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|from|[recipient](../resources/recipient.md)|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|hasAttachments|Boolean|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|importance|importance|**TODO: Add Description** Inherited from [message](../resources/message.md). Possible values are: `low`, `normal`, `high`.|
|inferenceClassification|inferenceClassificationType|**TODO: Add Description** Inherited from [message](../resources/message.md). Possible values are: `focused`, `other`.|
|internetMessageHeaders|[internetMessageHeader](../resources/internetmessageheader.md) collection|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|internetMessageId|String|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|isAllDay|Boolean|**TODO: Add Description** Inherited from [eventMessage](../resources/eventmessage.md)|
|isDelegated|Boolean|**TODO: Add Description** Inherited from [eventMessage](../resources/eventmessage.md)|
|isDeliveryReceiptRequested|Boolean|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|isDraft|Boolean|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|isOutOfDate|Boolean|**TODO: Add Description** Inherited from [eventMessage](../resources/eventmessage.md)|
|isRead|Boolean|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|isReadReceiptRequested|Boolean|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|location|[location](../resources/location.md)|**TODO: Add Description** Inherited from [eventMessage](../resources/eventmessage.md)|
|meetingMessageType|meetingMessageType|**TODO: Add Description** Inherited from [eventMessage](../resources/eventmessage.md). Possible values are: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTenativelyAccepted`, `meetingDeclined`.|
|parentFolderId|String|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|proposedNewTime|[timeSlot](../resources/timeslot.md)|**TODO: Add Description**|
|receivedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|**TODO: Add Description** Inherited from [eventMessage](../resources/eventmessage.md)|
|replyTo|[recipient](../resources/recipient.md) collection|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|responseType|responseType|**TODO: Add Description**. Possible values are: `none`, `organizer`, `tentativelyAccepted`, `accepted`, `declined`, `notResponded`.|
|sender|[recipient](../resources/recipient.md)|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|sentDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description** Inherited from [eventMessage](../resources/eventmessage.md)|
|subject|String|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|toRecipients|[recipient](../resources/recipient.md) collection|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|type|eventType|**TODO: Add Description** Inherited from [eventMessage](../resources/eventmessage.md). Possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.|
|uniqueBody|[itemBody](../resources/itembody.md)|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|webLink|String|**TODO: Add Description** Inherited from [message](../resources/message.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|attachments|[attachment](../resources/attachment.md) collection|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|event|[event](../resources/event.md)|**TODO: Add Description** Inherited from [eventMessage](../resources/eventmessage.md)|
|extensions|[extension](../resources/extension.md) collection|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|**TODO: Add Description** Inherited from [message](../resources/message.md)|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|**TODO: Add Description** Inherited from [message](../resources/message.md)|

## JSON representation
The following is a JSON representation of the resource.
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
  "inferenceClassification": "String",
  "flag": {
    "@odata.type": "microsoft.graph.followupFlag"
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
  "isOutOfDate": "Boolean",
  "isAllDay": "Boolean",
  "isDelegated": "Boolean",
  "proposedNewTime": {
    "@odata.type": "microsoft.graph.timeSlot"
  },
  "responseType": "String"
}
```

