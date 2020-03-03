---
title: "List workbookCommentReplies"
description: "List properties and relationships of the workbookCommentReply objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List workbookCommentReplies

Namespace: microsoft.graph

List properties and relationships of the [workbookCommentReply](../resources/workbookcommentreply.md) objects.

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
GET /me/drive/items/{driveItemId}/workbook/comments/{workbookCommentId}/replies
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workbookCommentReply](../resources/workbookcommentreply.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbookcommentreply"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/comments/{workbookCommentId}/replies
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbookcommentreply)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 231

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookCommentReply",
      "id": "e04be90f-e90f-e04b-0fe9-4be00fe94be0",
      "content": "Content value",
      "contentType": "Content Type value"
    }
  ]
}
```

