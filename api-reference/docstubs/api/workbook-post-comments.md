---
title: "Create comments"
description: "Create a new comments object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create comments

Namespace: microsoft.graph

Create a new comments object.

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
POST /invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/comments
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [workbookComment](../resources/workbookcomment.md) object.

The following table shows the properties that are required when you create the [workbookComment](../resources/workbookcomment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|content|String|**TODO: Add Description**|
|contentType|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [workbookComment](../resources/workbookcomment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_workbookcomment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/drive/items/{driveItemId}/workbook/comments
Content-Type: application/json
Content-length: 128

{
  "@odata.type": "#microsoft.graph.workbookComment",
  "content": "Content value",
  "contentType": "Content Type value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookcomment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.workbookComment",
  "id": "ff04e299-e299-ff04-99e2-04ff99e204ff",
  "content": "Content value",
  "contentType": "Content Type value"
}
```

