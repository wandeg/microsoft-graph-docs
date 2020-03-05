---
title: "Update eventMessage"
description: "Update the properties of a eventMessage object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update eventMessage

Namespace: microsoft.graph

Update the properties of a [eventMessage](../resources/eventmessage.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH ** Entity URI for microsoft.graph.eventMessage not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

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
|inferenceClassification|Enumeration| Inherited from [message](../resources/message.md). Possible values are: `focused`, `other`.|
|flag|[followupFlag](../resources/followupflag.md)| Inherited from [message](../resources/message.md)|
|meetingMessageType|Enumeration|. Possible values are: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTenativelyAccepted`, `meetingDeclined`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [eventMessage](../resources/eventmessage.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_eventmessage"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.eventMessage not found
Content-type: application/json
Content-length: 2231

{
  "@odata.type": "#microsoft.graph.eventMessage",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "receivedDateTime": "2017-01-01T00:02:50.2294959+03:00",
  "sentDateTime": "2017-01-01T00:02:05.1031932+03:00",
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
  "inferenceClassification": "String",
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
  "meetingMessageType": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2401

{
  "@odata.type": "#microsoft.graph.eventMessage",
  "id": "057a3b6c-3b6c-057a-6c3b-7a056c3b7a05",
  "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
  "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "receivedDateTime": "2017-01-01T00:02:50.2294959+03:00",
  "sentDateTime": "2017-01-01T00:02:05.1031932+03:00",
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
  "inferenceClassification": "String",
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
  "meetingMessageType": "String"
}
```

