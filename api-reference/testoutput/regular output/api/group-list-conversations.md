---
title: "List conversations"
description: "Get the conversations from the conversations navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List conversations

Namespace: microsoft.graph

Get the conversations from the conversations navigation property.

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
GET /groups/{groupsId}/conversations
GET /me/joinedTeams/{groupId}/conversations
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [conversation](../resources/conversation.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_conversation"
}
-->
``` http
GET https://graph.microsoft.com/localtest/groups/{groupsId}/conversations
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.conversation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 378

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.conversation",
      "id": "9db8ecd0-ecd0-9db8-d0ec-b89dd0ecb89d",
      "topic": "Topic value",
      "hasAttachments": true,
      "lastDeliveredDateTime": "2017-01-01T00:02:45.7138413+03:00",
      "uniqueSenders": [
        "Unique Senders value"
      ],
      "preview": "Preview value"
    }
  ]
}
```

