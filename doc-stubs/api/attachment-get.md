---
title: "Get attachment"
description: "Read the properties and relationships of an attachment object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get attachment

Namespace: microsoft.graph

Read the properties and relationships of an [attachment](../resources/attachment.md) object.

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
GET /me/messages/{messageId}/attachments/{attachmentId}
GET /me/messages/{messageId}/event/attachments/{attachmentId}
GET /users/{usersId}/messages/{messageId}/attachments/{attachmentId}
GET /users/{usersId}/messages/{messageId}/event/attachments/{attachmentId}
GET /groups/{groupsId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/attachments/{attachmentId}
GET /me/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/tasks/{outlookTaskId}/attachments/{attachmentId}
GET /users/{usersId}/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/tasks/{outlookTaskId}/attachments/{attachmentId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [attachment](../resources/attachment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_attachment"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/messages/{messageId}/attachments/{attachmentId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.attachment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.attachment",
    "id": "fb195bad-5bad-fb19-ad5b-19fbad5b19fb",
    "lastModifiedDateTime": "String (timestamp)",
    "name": "String",
    "contentType": "String",
    "size": "Integer",
    "isInline": "Boolean"
  }
}
```

