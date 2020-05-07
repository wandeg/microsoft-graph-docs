---
title: "message: delta"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# delta

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
GET /me/messages/delta
GET /users/{usersId}/messages/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Function parameters
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a [message](../resources/message.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "message_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/messages/delta
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.message)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.message",
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
      "mentionsPreview": {
        "@odata.type": "microsoft.graph.mentionsPreview"
      },
      "inferenceClassification": "String",
      "unsubscribeData": [
        "String"
      ],
      "unsubscribeEnabled": "Boolean",
      "flag": {
        "@odata.type": "microsoft.graph.followupFlag"
      }
    }
  ]
}
```

