---
title: "List chats"
description: "Get the chats from the chats navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List chats

Namespace: microsoft.graph

Get the chats from the chats navigation property.

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
GET /me/chats
GET /users/{usersId}/chats
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
If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_chat"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/chats
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.chat)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.chat",
      "id": "3024901c-901c-3024-1c90-24301c902430",
      "topic": "Topic value",
      "createdDateTime": "2017-01-01T00:00:27.4994223+03:00",
      "lastUpdatedDateTime": "2016-12-31T23:57:05.0114435+03:00"
    }
  ]
}
```

