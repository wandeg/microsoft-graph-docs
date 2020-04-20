---
title: "Get chat"
description: "Read properties and relationships of a chat object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get chat

Namespace: microsoft.graph

Read properties and relationships of a [chat](../resources/chat.md) object.

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
GET /chats/{chatsId}
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
If successful, this method returns a `200 OK` response code and a [chat](../resources/chat.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_chat"
}
-->
``` http
GET https://graph.microsoft.com/beta/chats/{chatsId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.chat",
    "id": "c30e7705-7705-c30e-0577-0ec305770ec3",
    "topic": "Topic value",
    "createdDateTime": "2016-12-31T23:57:02.5240758+03:00",
    "lastUpdatedDateTime": "2016-12-31T23:58:30.1015683+03:00"
  }
}
```

