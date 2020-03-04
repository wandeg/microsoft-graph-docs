---
title: "List conversationThreads"
description: "List properties and relationships of the conversationThread objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List conversationThreads

Namespace: microsoft.graph

List properties and relationships of the [conversationThread](../resources/conversationthread.md) objects.

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
GET /groups/{groupsId}/threads
GET /me/joinedTeams/{groupId}/threads
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

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_conversationthread"
}
-->
``` http
GET https://graph.microsoft.com/localtest/groups/{groupsId}/threads
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
      "id": "3a751750-1750-3a75-5017-753a5017753a",
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
      "lastDeliveredDateTime": "2017-01-01T00:01:15.4160233+03:00",
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

