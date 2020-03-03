---
title: "Update documentCommentReply"
description: "Update the properties of a documentCommentReply object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update documentCommentReply

Update the properties of a [documentCommentReply](../resources/documentcommentreply.md) object.

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
PATCH /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/document/comments/{documentCommentId}/replies/{documentCommentReplyId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [documentCommentReply](../resources/documentCommentReply.md) object.

The following table shows the properties that are required when you create the [documentCommentReply](../resources/documentcommentreply.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|content|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [documentCommentReply](../resources/documentcommentreply.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_documentcommentreply"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/document/comments/{documentCommentId}/replies/{documentCommentReplyId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 142

{
  "@odata.type": "#microsoft.graph.documentCommentReply",
  "id": "9163fc2b-fc2b-9163-2bfc-63912bfc6391",
  "content": "Content value"
}
```

