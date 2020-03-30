---
title: "Update outlookTaskFolder"
description: "Update the properties of a outlookTaskFolder object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update outlookTaskFolder

Namespace: microsoft.graph

Update the properties of a [outlookTaskFolder](../resources/outlooktaskfolder.md) object.

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
PATCH /me/outlook/taskFolders/{outlookTaskFolderId}
PATCH /me/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [outlookTaskFolder](../resources/outlooktaskfolder.md) object.

The following table shows the properties that are required when you create the [outlookTaskFolder](../resources/outlooktaskfolder.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|changeKey|String||
|name|String||
|isDefaultFolder|Boolean||
|parentGroupKey|Guid||



## Response
If successful, this method returns a `200 OK` response code and an updated [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_outlooktaskfolder"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/outlook/taskFolders/{outlookTaskFolderId}
Content-type: application/json
Content-length: 209

{
  "@odata.type": "#microsoft.graph.outlookTaskFolder",
  "changeKey": "Change Key value",
  "name": "Name value",
  "isDefaultFolder": true,
  "parentGroupKey": "6ed14fba-4fba-6ed1-ba4f-d16eba4fd16e"
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
Content-Length: 258

{
  "@odata.type": "#microsoft.graph.outlookTaskFolder",
  "id": "ea1c2771-2771-ea1c-7127-1cea71271cea",
  "changeKey": "Change Key value",
  "name": "Name value",
  "isDefaultFolder": true,
  "parentGroupKey": "6ed14fba-4fba-6ed1-ba4f-d16eba4fd16e"
}
```

