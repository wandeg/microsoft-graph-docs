---
title: "Create taskFolders"
description: "Create a new taskFolders object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create taskFolders

Namespace: microsoft.graph

Create a new taskFolders object.

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
POST /me/outlook/taskFolders
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [outlookTaskFolder](../resources/outlooktaskfolder.md) object.

The following table shows the properties that are required when you create the [outlookTaskFolder](../resources/outlooktaskfolder.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|changeKey|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|isDefaultFolder|Boolean|**TODO: Add Description**|
|parentGroupKey|Guid|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/outlook/taskFolders
Content-Type: application/json
Content-length: 209

{
  "@odata.type": "#microsoft.graph.outlookTaskFolder",
  "changeKey": "Change Key value",
  "name": "Name value",
  "isDefaultFolder": true,
  "parentGroupKey": "7c1f1401-1401-7c1f-0114-1f7c01141f7c"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlooktaskfolder"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.outlookTaskFolder",
  "id": "ef51946b-946b-ef51-6b94-51ef6b9451ef",
  "changeKey": "Change Key value",
  "name": "Name value",
  "isDefaultFolder": true,
  "parentGroupKey": "7c1f1401-1401-7c1f-0114-1f7c01141f7c"
}
```

