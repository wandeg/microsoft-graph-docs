---
title: "outlookTask: complete"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# complete

Namespace: microsoft.graph

**TODO: Add Description**

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
POST /invitations/{invitationsId}/invitedUser/outlook/tasks/{outlookTaskId}/complete
POST /invitations/{invitationsId}/invitedUser/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/tasks/{outlookTaskId}/complete
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this action returns a `200 OK` response code and a [outlookTask](../resources/outlooktask.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "outlooktask_complete"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/outlook/tasks/{outlookTaskId}/complete
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.outlooktask)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.outlookTask",
      "id": "4d8492c0-92c0-4d84-c092-844dc092844d",
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
      "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
      "changeKey": "Change Key value",
      "categories": [
        "Categories value"
      ],
      "assignedTo": "Assigned To value",
      "body": {
        "@odata.type": "microsoft.graph.itemBody"
      },
      "completedDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "dueDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "hasAttachments": true,
      "importance": "String",
      "isReminderOn": true,
      "owner": "Owner value",
      "parentFolderId": "Parent Folder Id value",
      "recurrence": {
        "@odata.type": "microsoft.graph.patternedRecurrence"
      },
      "reminderDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "sensitivity": "String",
      "startDateTime": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "status": "String",
      "subject": "Subject value"
    }
  ]
}
```

