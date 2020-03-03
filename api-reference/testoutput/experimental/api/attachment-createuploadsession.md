---
title: "createUploadSession"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# createUploadSession



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
POST /me/messages/{messageId}/attachments/createUploadSession
POST /me/messages/{messageId}/event/attachments/createUploadSession
POST /me/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/tasks/{outlookTaskId}/attachments/createUploadSession
POST /me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/attachments/createUploadSession
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|AttachmentItem|[attachmentItem](../resources/attachmentItem.md)||



## Response
If successful, this action returns a `200 OK` response code and a [uploadSession](../resources/uploadSession.md) in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "attachment_createuploadsession"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/me/messages/{messageId}/attachments/createUploadSession

Content-type: application/json
Content-length: 134

{
  "AttachmentItem": {
    "@odata.type": "microsoft.graph.attachmentItem",
    "attachmentType": "String",
    "size": 4
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.uploadsession"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 75

{
  "value": {
    "@odata.type": "microsoft.graph.uploadSession"
  }
}
```

