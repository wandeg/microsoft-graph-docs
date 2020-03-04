---
title: "List eventMessages"
description: "List properties and relationships of the eventMessage objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List eventMessages

Namespace: microsoft.graph

List properties and relationships of the [eventMessage](../resources/eventmessage.md) objects.

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
GET ** Collection URI for microsoft.graph.eventMessage not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [eventMessage](../resources/eventmessage.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_eventmessage"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.eventMessage not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.eventmessage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2776

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.eventMessage",
      "id": "641592e9-92e9-6415-e992-1564e9921564",
      "createdDateTime": "2017-01-01T00:01:25.3917672+03:00",
      "lastModifiedDateTime": "2016-12-31T23:58:55.6908839+03:00",
      "changeKey": "Change Key value",
      "categories": [
        "Categories value"
      ],
      "receivedDateTime": "2017-01-01T00:02:17.8932513+03:00",
      "sentDateTime": "2017-01-01T00:01:02.4648747+03:00",
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
  ]
}
```

