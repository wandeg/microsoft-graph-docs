---
title: "List chats"
description: "Get the chats from the chats navigation property."
author: ""
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
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

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
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [chat](../resources/chat.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_chat"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/chats
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.chat)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 297

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.chat",
      "id": "b4749289-9289-b474-8992-74b4899274b4",
      "topic": "Topic value",
      "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
      "lastUpdatedDateTime": "2016-12-31T23:59:55.7493178+03:00"
    }
  ]
}
```

