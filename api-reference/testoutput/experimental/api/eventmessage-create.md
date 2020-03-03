---
title: "Create eventMessage"
description: "Create a new eventMessage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create eventMessage

Namespace: microsoft.graph

Create a new [eventMessage](../resources/eventmessage.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST ** Collection URI for microsoft.graph.eventMessage not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [eventMessage](../resources/eventmessage.md) object.

The following table shows the properties that are required when you create the [eventMessage](../resources/eventmessage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|changeKey|String| Inherited from [outlookItem](../resources/outlookitem.md)|
|categories|String collection| Inherited from [outlookItem](../resources/outlookitem.md)|
|receivedDateTime|DateTimeOffset| Inherited from [message](../resources/message.md)|
|sentDateTime|DateTimeOffset| Inherited from [message](../resources/message.md)|
|hasAttachments|Boolean| Inherited from [message](../resources/message.md)|
|internetMessageId|String| Inherited from [message](../resources/message.md)|
|internetMessageHeaders|[internetMessageHeader](../resources/internetmessageheader.md) collection| Inherited from [message](../resources/message.md)|
|subject|String| Inherited from [message](../resources/message.md)|
|body|[itemBody](../resources/itembody.md)| Inherited from [message](../resources/message.md)|
|bodyPreview|String| Inherited from [message](../resources/message.md)|
|importance|Enumeration| Inherited from [message](../resources/message.md). Possible values are: `low`, `normal`, `high`.|
|parentFolderId|String| Inherited from [message](../resources/message.md)|
|sender|[recipient](../resources/recipient.md)| Inherited from [message](../resources/message.md)|
|from|[recipient](../resources/recipient.md)| Inherited from [message](../resources/message.md)|
|toRecipients|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|ccRecipients|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|bccRecipients|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|replyTo|[recipient](../resources/recipient.md) collection| Inherited from [message](../resources/message.md)|
|conversationId|String| Inherited from [message](../resources/message.md)|
|conversationIndex|Binary| Inherited from [message](../resources/message.md)|
|uniqueBody|[itemBody](../resources/itembody.md)| Inherited from [message](../resources/message.md)|
|isDeliveryReceiptRequested|Boolean| Inherited from [message](../resources/message.md)|
|isReadReceiptRequested|Boolean| Inherited from [message](../resources/message.md)|
|isRead|Boolean| Inherited from [message](../resources/message.md)|
|isDraft|Boolean| Inherited from [message](../resources/message.md)|
|webLink|String| Inherited from [message](../resources/message.md)|
|mentionsPreview|[mentionsPreview](../resources/mentionspreview.md)| Inherited from [message](../resources/message.md)|
|inferenceClassification|Enumeration| Inherited from [message](../resources/message.md). Possible values are: `focused`, `other`.|
|unsubscribeData|String collection| Inherited from [message](../resources/message.md)|
|unsubscribeEnabled|Boolean| Inherited from [message](../resources/message.md)|
|flag|[followupFlag](../resources/followupflag.md)| Inherited from [message](../resources/message.md)|
|meetingMessageType|Enumeration|. Possible values are: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTentativelyAccepted`, `meetingDeclined`.|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|endDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|location|[location](../resources/location.md)||
|type|Enumeration|. Possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)||
|isOutOfDate|Boolean||
|isAllDay|Boolean||
|isDelegated|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [eventMessage](../resources/eventmessage.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_eventmessage_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.eventMessage not found
Content-type: application/json
Content-length: 4210

{
  "@odata.type": "#microsoft.graph.eventMessage",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "receivedDateTime": "2016-12-31T23:59:19.9005871+03:00",
  "sentDateTime": "2016-12-31T23:58:01.3361491+03:00",
  "hasAttachments": true,
  "internetMessageId": "Internet Message Id value",
  "internetMessageHeaders": [
    {
      "@odata.type": "microsoft.graph.internetMessageHeader",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "subject": "Subject value",
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "Content value"
  },
  "bodyPreview": "Body Preview value",
  "importance": "String",
  "parentFolderId": "Parent Folder Id value",
  "sender": {
    "@odata.type": "microsoft.graph.recipient",
    "emailAddress": {
      "@odata.type": "microsoft.graph.emailAddress",
      "address": "Address value"
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
  "conversationId": "Conversation Id value",
  "conversationIndex": "Y29udmVyc2F0aW9uSW5kZXg=",
  "uniqueBody": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "isDeliveryReceiptRequested": true,
  "isReadReceiptRequested": true,
  "isRead": true,
  "isDraft": true,
  "webLink": "Web Link value",
  "mentionsPreview": {
    "@odata.type": "microsoft.graph.mentionsPreview",
    "isMentioned": true
  },
  "inferenceClassification": "String",
  "unsubscribeData": [
    "Unsubscribe Data value"
  ],
  "unsubscribeEnabled": true,
  "flag": {
    "@odata.type": "microsoft.graph.followupFlag",
    "completedDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone",
      "dateTime": "Date Time value",
      "timeZone": "Time Zone value"
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
    "@odata.type": "microsoft.graph.location",
    "displayName": "Display Name value",
    "locationEmailAddress": "Location Email Address value",
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress",
      "type": "String",
      "postOfficeBox": "Post Office Box value",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryOrRegion": "Country Or Region value",
      "postalCode": "Postal Code value"
    },
    "coordinates": {
      "@odata.type": "microsoft.graph.outlookGeoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double",
      "accuracy": "Double",
      "altitudeAccuracy": "Double"
    },
    "locationUri": "Location Uri value",
    "locationType": "String",
    "uniqueId": "Unique Id value",
    "uniqueIdType": "String"
  },
  "type": "String",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence",
    "pattern": {
      "@odata.type": "microsoft.graph.recurrencePattern",
      "type": "String",
      "interval": 8,
      "month": 5,
      "dayOfMonth": 10,
      "daysOfWeek": [
        "String"
      ],
      "firstDayOfWeek": "String",
      "index": "String"
    },
    "range": {
      "@odata.type": "microsoft.graph.recurrenceRange",
      "type": "String",
      "startDate": "Date",
      "endDate": "Date",
      "recurrenceTimeZone": "Recurrence Time Zone value",
      "numberOfOccurrences": 3
    }
  },
  "isOutOfDate": true,
  "isAllDay": true,
  "isDelegated": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.eventmessage"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4381

{
  "@odata.type": "#microsoft.graph.eventMessage",
  "id": "cccde51b-e51b-cccd-1be5-cdcc1be5cdcc",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "receivedDateTime": "2016-12-31T23:59:19.9005871+03:00",
  "sentDateTime": "2016-12-31T23:58:01.3361491+03:00",
  "hasAttachments": true,
  "internetMessageId": "Internet Message Id value",
  "internetMessageHeaders": [
    {
      "@odata.type": "microsoft.graph.internetMessageHeader",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "subject": "Subject value",
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "Content value"
  },
  "bodyPreview": "Body Preview value",
  "importance": "String",
  "parentFolderId": "Parent Folder Id value",
  "sender": {
    "@odata.type": "microsoft.graph.recipient",
    "emailAddress": {
      "@odata.type": "microsoft.graph.emailAddress",
      "address": "Address value"
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
  "conversationId": "Conversation Id value",
  "conversationIndex": "Y29udmVyc2F0aW9uSW5kZXg=",
  "uniqueBody": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "isDeliveryReceiptRequested": true,
  "isReadReceiptRequested": true,
  "isRead": true,
  "isDraft": true,
  "webLink": "Web Link value",
  "mentionsPreview": {
    "@odata.type": "microsoft.graph.mentionsPreview",
    "isMentioned": true
  },
  "inferenceClassification": "String",
  "unsubscribeData": [
    "Unsubscribe Data value"
  ],
  "unsubscribeEnabled": true,
  "flag": {
    "@odata.type": "microsoft.graph.followupFlag",
    "completedDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone",
      "dateTime": "Date Time value",
      "timeZone": "Time Zone value"
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
    "@odata.type": "microsoft.graph.location",
    "displayName": "Display Name value",
    "locationEmailAddress": "Location Email Address value",
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress",
      "type": "String",
      "postOfficeBox": "Post Office Box value",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryOrRegion": "Country Or Region value",
      "postalCode": "Postal Code value"
    },
    "coordinates": {
      "@odata.type": "microsoft.graph.outlookGeoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double",
      "accuracy": "Double",
      "altitudeAccuracy": "Double"
    },
    "locationUri": "Location Uri value",
    "locationType": "String",
    "uniqueId": "Unique Id value",
    "uniqueIdType": "String"
  },
  "type": "String",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence",
    "pattern": {
      "@odata.type": "microsoft.graph.recurrencePattern",
      "type": "String",
      "interval": 8,
      "month": 5,
      "dayOfMonth": 10,
      "daysOfWeek": [
        "String"
      ],
      "firstDayOfWeek": "String",
      "index": "String"
    },
    "range": {
      "@odata.type": "microsoft.graph.recurrenceRange",
      "type": "String",
      "startDate": "Date",
      "endDate": "Date",
      "recurrenceTimeZone": "Recurrence Time Zone value",
      "numberOfOccurrences": 3
    }
  },
  "isOutOfDate": true,
  "isAllDay": true,
  "isDelegated": true
}
```

