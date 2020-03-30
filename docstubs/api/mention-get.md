---
title: "Get mention"
description: "Read properties and relationships of the mention object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get mention

Namespace: microsoft.graph

Read properties and relationships of the [mention](../resources/mention.md) object.

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
GET /me/messages/{messageId}/mentions/{mentionId}
GET /me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/mentions/{mentionId}
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
If successful, this method returns a `200 OK` response code and [mention](../resources/mention.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_mention"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/messages/{messageId}/mentions/{mentionId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mention"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 644

{
  "value": {
    "@odata.type": "#microsoft.graph.mention",
    "id": "98c44b8b-4b8b-98c4-8b4b-c4988b4bc498",
    "mentioned": {
      "@odata.type": "microsoft.graph.emailAddress",
      "name": "Name value",
      "address": "Address value"
    },
    "mentionText": "Mention Text value",
    "clientReference": "Client Reference value",
    "createdBy": {
      "@odata.type": "microsoft.graph.emailAddress"
    },
    "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
    "serverCreatedDateTime": "2017-01-01T00:01:34.8394338+03:00",
    "deepLink": "Deep Link value",
    "application": "Application value"
  }
}
```

