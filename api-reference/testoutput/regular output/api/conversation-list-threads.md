---
title: "List threads"
description: "Get the conversationThreads from the threads navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List threads

Namespace: microsoft.graph

Get the conversationThreads from the threads navigation property.

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
GET /me/joinedTeams/{groupId}/conversations/{conversationId}/threads
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [conversationThread](../resources/conversationthread.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/joinedTeams/{groupId}/conversations/{conversationId}/threads
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.conversationthread)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 809

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.conversationThread",
      "id": "6acc11f7-11f7-6acc-f711-cc6af711cc6a",
      "toRecipients": [
        {
          "@odata.type": "microsoft.graph.recipient",
          "emailAddress": {
            "@odata.type": "microsoft.graph.emailAddress",
            "name": "Name value",
            "address": "Address value"
          }
        }
      ],
      "topic": "Topic value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "2017-01-01T00:02:45.7138413+03:00",
      "uniqueSenders": [
        "Unique Senders value"
      ],
      "ccRecipients": [
        {
          "@odata.type": "microsoft.graph.recipient"
        }
      ],
      "preview": "Preview value",
      "isLocked": true
    }
  ]
}
```

