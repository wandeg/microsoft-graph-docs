---
title: "Add taskFolders"
description: "Add taskFolders by posting to the taskFolders collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add taskFolders

Namespace: microsoft.graph

Add taskFolders by posting to the taskFolders collection.

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
POST /me/outlook/taskFolders/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskfolder_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/outlook/taskFolders
Content-type: application/json
Content-length: 209

{
  "@odata.type": "#microsoft.graph.outlookTaskFolder",
  "changeKey": "Change Key value",
  "name": "Name value",
  "isDefaultFolder": true,
  "parentGroupKey": "bb6a0632-0632-bb6a-3206-6abb32066abb"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlooktaskfolder"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 258

{
  "@odata.type": "#microsoft.graph.outlookTaskFolder",
  "id": "cd330c2c-0c2c-cd33-2c0c-33cd2c0c33cd",
  "changeKey": "Change Key value",
  "name": "Name value",
  "isDefaultFolder": true,
  "parentGroupKey": "bb6a0632-0632-bb6a-3206-6abb32066abb"
}
```

