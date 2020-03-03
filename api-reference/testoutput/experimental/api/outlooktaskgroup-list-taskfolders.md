---
title: "List taskFolders"
description: "Get the outlookTaskFolders from the taskFolders navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List taskFolders

Get the outlookTaskFolders from the taskFolders navigation property.

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
GET /me/outlook/taskGroups/{outlookTaskGroupId}/taskFolders
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/me/outlook/taskGroups/{outlookTaskGroupId}/taskFolders
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.outlooktaskfolder)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 315

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.outlookTaskFolder",
      "id": "a33aa597-a597-a33a-97a5-3aa397a53aa3",
      "changeKey": "Change Key value",
      "name": "Name value",
      "isDefaultFolder": true,
      "parentGroupKey": "b2d07fae-7fae-b2d0-ae7f-d0b2ae7fd0b2"
    }
  ]
}
```

