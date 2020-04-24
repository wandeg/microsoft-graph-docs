---
title: "Update attachments"
description: "Update the properties of an attachments object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update attachments

Namespace: microsoft.graph

Update the properties of an attachments object.

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
PATCH /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/attachments
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [attachment](../resources/attachment.md) object.

The following table shows the properties that are required when you create the [attachment](../resources/attachment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|contentType|String|**TODO: Add Description**|
|size|Int32|**TODO: Add Description**|
|isInline|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [attachment](../resources/attachment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_attachments"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/attachments
Content-Type: application/json
Content-length: 152

{
  "@odata.type": "#microsoft.graph.attachment",
  "name": "Name value",
  "contentType": "Content Type value",
  "size": 4,
  "isInline": true
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.attachment",
  "id": "17da23c1-23c1-17da-c123-da17c123da17",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "name": "Name value",
  "contentType": "Content Type value",
  "size": 4,
  "isInline": true
}
```

