---
title: "user: sendMail"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# sendMail

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /me/sendMail
POST /users/{usersId}/sendMail
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|Message|[message](../resources/message.md)|**TODO: Add Description**|
|SaveToSentItems|Boolean|**TODO: Add Description**|



## Response
If successful, this action returns a `204 No Content` response code.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "user_sendmail"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/sendMail

Content-Type: application/json
Content-length: 2308

{
  "Message": {
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
        "@odata.type": "microsoft.graph.internetMessageHeader"
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
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "dueDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "startDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "flagStatus": "String"
    }
  },
  "SaveToSentItems": true
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

