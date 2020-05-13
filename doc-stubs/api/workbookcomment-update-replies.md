---
title: "Update replies"
description: "Update the properties of a replies object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update replies

Namespace: microsoft.graph

Update the properties of a replies object.

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
PATCH /workbooks/{workbooksId}/workbook/comments/{workbookCommentId}/replies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [workbookCommentReply](../resources/workbookcommentreply.md) object.

The following table shows the properties that are required when you create the [workbookCommentReply](../resources/workbookcommentreply.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|content|String|**TODO: Add Description**|
|contentType|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [workbookCommentReply](../resources/workbookcommentreply.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_replies"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/workbooks/{workbooksId}/workbook/comments/{workbookCommentId}/replies
Content-Type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.workbookCommentReply",
  "content": "String",
  "contentType": "String"
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
  "@odata.type": "#microsoft.graph.workbookCommentReply",
  "id": "5ec76225-6225-5ec7-2562-c75e2562c75e",
  "content": "String",
  "contentType": "String"
}
```

