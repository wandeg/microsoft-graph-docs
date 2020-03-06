---
title: "Add replies"
description: "Add replies by posting to the replies collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add replies

Namespace: microsoft.graph

Add replies by posting to the replies collection.

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
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/document/comments/{documentCommentId}/replies/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [documentCommentReply](../resources/documentcommentreply.md) object.

The following table shows the properties that are required when you create the [documentCommentReply](../resources/documentcommentreply.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|content|String||



## Response
If successful, this method returns a `201 Created` response code and a [documentCommentReply](../resources/documentcommentreply.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_documentcommentreply_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/document/comments/{documentCommentId}/replies
Content-type: application/json
Content-length: 93

{
  "@odata.type": "#microsoft.graph.documentCommentReply",
  "content": "Content value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.documentcommentreply"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 142

{
  "@odata.type": "#microsoft.graph.documentCommentReply",
  "id": "5a6bba21-ba21-5a6b-21ba-6b5a21ba6b5a",
  "content": "Content value"
}
```

