---
title: "Get outlookTaskFolder"
description: "Read properties and relationships of the outlookTaskFolder object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get outlookTaskFolder

Namespace: microsoft.graph

Read properties and relationships of the [outlookTaskFolder](../resources/outlooktaskfolder.md) object.

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
GET /me/outlook/taskFolders/{outlookTaskFolderId}
GET /me/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/{outlookTaskFolderId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 289

{
  "value": {
    "@odata.type": "#microsoft.graph.outlookTaskFolder",
    "id": "6eb6c8db-c8db-6eb6-dbc8-b66edbc8b66e",
    "changeKey": "Change Key value",
    "name": "Name value",
    "isDefaultFolder": true,
    "parentGroupKey": "bd124508-4508-bd12-0845-12bd084512bd"
  }
}
```

