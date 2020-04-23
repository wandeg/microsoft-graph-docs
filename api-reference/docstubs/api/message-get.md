---
title: "Get message"
description: "Read the properties and relationships of a message object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get message

Namespace: microsoft.graph

Read the properties and relationships of a [message](../resources/message.md) object.

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
GET /me/messages/{messageId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [message](../resources/message.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_message"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/messages/{messageId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.message",
    "id": "fa8eb03b-b03b-fa8e-3bb0-8efa3bb08efa",
    "createdDateTime": "2017-01-01T00:02:24.9669049+03:00",
    "lastModifiedDateTime": "2017-01-01T00:02:46.687785+03:00",
    "changeKey": "Change Key value",
    "categories": [
      "Categories value"
    ],
    "receivedDateTime": "2017-01-01T00:02:01.0790636+03:00",
    "sentDateTime": "2016-12-31T23:57:58.8506721+03:00",
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
    }
  }
}
```

