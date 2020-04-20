---
title: "Update messages"
description: "Update the properties of a messages object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update messages

Namespace: microsoft.graph

Update the properties of a messages object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/messages
PATCH /users/{usersId}/messages
PATCH /invitations/{invitationsId}/invitedUser/messages
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [message](../resources/message.md) object.

The following table shows the properties that are required when you create the [message](../resources/message.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|changeKey|String|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|categories|String collection|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|receivedDateTime|DateTimeOffset|**TODO: Add Description**|
|sentDateTime|DateTimeOffset|**TODO: Add Description**|
|hasAttachments|Boolean|**TODO: Add Description**|
|internetMessageId|String|**TODO: Add Description**|
|internetMessageHeaders|[internetMessageHeader](../resources/internetmessageheader.md) collection|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|
|body|[itemBody](../resources/itembody.md)|**TODO: Add Description**|
|bodyPreview|String|**TODO: Add Description**|
|importance|importance|**TODO: Add Description**. Possible values are: `low`, `normal`, `high`.|
|parentFolderId|String|**TODO: Add Description**|
|sender|[recipient](../resources/recipient.md)|**TODO: Add Description**|
|from|[recipient](../resources/recipient.md)|**TODO: Add Description**|
|toRecipients|[recipient](../resources/recipient.md) collection|**TODO: Add Description**|
|ccRecipients|[recipient](../resources/recipient.md) collection|**TODO: Add Description**|
|bccRecipients|[recipient](../resources/recipient.md) collection|**TODO: Add Description**|
|replyTo|[recipient](../resources/recipient.md) collection|**TODO: Add Description**|
|conversationId|String|**TODO: Add Description**|
|conversationIndex|Binary|**TODO: Add Description**|
|uniqueBody|[itemBody](../resources/itembody.md)|**TODO: Add Description**|
|isDeliveryReceiptRequested|Boolean|**TODO: Add Description**|
|isReadReceiptRequested|Boolean|**TODO: Add Description**|
|isRead|Boolean|**TODO: Add Description**|
|isDraft|Boolean|**TODO: Add Description**|
|webLink|String|**TODO: Add Description**|
|mentionsPreview|[mentionsPreview](../resources/mentionspreview.md)|**TODO: Add Description**|
|inferenceClassification|inferenceClassificationType|**TODO: Add Description**. Possible values are: `focused`, `other`.|
|unsubscribeData|String collection|**TODO: Add Description**|
|unsubscribeEnabled|Boolean|**TODO: Add Description**|
|flag|[followupFlag](../resources/followupflag.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [message](../resources/message.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_messages"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/messages
Content-Type: application/json
Content-length: 2392

{
  "@odata.type": "#microsoft.graph.message",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "receivedDateTime": "2016-12-31T23:59:43.2782812+03:00",
  "sentDateTime": "2017-01-01T00:00:09.9084378+03:00",
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
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.message",
  "id": "b914f601-f601-b914-01f6-14b901f614b9",
  "createdDateTime": "2016-12-31T23:57:02.5240758+03:00",
  "lastModifiedDateTime": "2017-01-01T00:01:44.3371159+03:00",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "receivedDateTime": "2016-12-31T23:59:43.2782812+03:00",
  "sentDateTime": "2017-01-01T00:00:09.9084378+03:00",
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
  }
}
```

