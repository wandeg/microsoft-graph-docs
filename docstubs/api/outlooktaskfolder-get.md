---
title: "Get outlookTaskFolder"
description: "Read properties and relationships of an outlookTaskFolder object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get outlookTaskFolder

Namespace: microsoft.graph

Read properties and relationships of an [outlookTaskFolder](../resources/outlooktaskfolder.md) object.

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
GET /invitations/{invitationsId}/invitedUser/outlook/taskFolders/{outlookTaskFolderId}
GET /invitations/{invitationsId}/invitedUser/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and an [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/outlook/taskFolders/{outlookTaskFolderId}
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
{
  "value": {
    "@odata.type": "#microsoft.graph.outlookTaskFolder",
    "id": "9b6848fc-48fc-9b68-fc48-689bfc48689b",
    "changeKey": "Change Key value",
    "name": "Name value",
    "isDefaultFolder": true,
    "parentGroupKey": "0fdd472d-472d-0fdd-2d47-dd0f2d47dd0f"
  }
}
```

