---
title: "Add tasks"
description: "Add tasks by posting to the tasks collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add tasks

Namespace: microsoft.graph

Add tasks by posting to the tasks collection.

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
POST /me/outlook/tasks/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [outlookTask](../resources/outlooktask.md) object.

The following table shows the properties that are required when you create the [outlookTask](../resources/outlooktask.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [outlookItem](../resources/outlookitem.md)|
|changeKey|String| Inherited from [outlookItem](../resources/outlookitem.md)|
|categories|String collection| Inherited from [outlookItem](../resources/outlookitem.md)|
|assignedTo|String||
|body|[itemBody](../resources/itembody.md)||
|completedDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|hasAttachments|Boolean||
|importance|Enumeration|. Possible values are: `low`, `normal`, `high`.|
|isReminderOn|Boolean||
|owner|String||
|parentFolderId|String||
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)||
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|sensitivity|Enumeration|. Possible values are: `normal`, `personal`, `private`, `confidential`.|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)||
|status|Enumeration|. Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.|
|subject|String||



## Response
If successful, this method returns a `201 Created` response code and a [outlookTask](../resources/outlooktask.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_outlooktask_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/outlook/tasks
Content-type: application/json
Content-length: 1570

{
  "@odata.type": "#microsoft.graph.outlookTask",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "assignedTo": "Assigned To value",
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "Content value"
  },
  "completedDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "Date Time value",
    "timeZone": "Time Zone value"
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
    "@odata.type": "microsoft.graph.patternedRecurrence",
    "pattern": {
      "@odata.type": "microsoft.graph.recurrencePattern",
      "type": "String",
      "interval": 8,
      "month": 5,
      "dayOfMonth": 10,
      "daysOfWeek": [
        "String"
      ],
      "firstDayOfWeek": "String",
      "index": "String"
    },
    "range": {
      "@odata.type": "microsoft.graph.recurrenceRange",
      "type": "String",
      "startDate": "Date",
      "endDate": "Date",
      "recurrenceTimeZone": "Recurrence Time Zone value",
      "numberOfOccurrences": 3
    }
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlooktask"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1742

{
  "@odata.type": "#microsoft.graph.outlookTask",
  "id": "23d09373-9373-23d0-7393-d0237393d023",
  "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
  "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00",
  "changeKey": "Change Key value",
  "categories": [
    "Categories value"
  ],
  "assignedTo": "Assigned To value",
  "body": {
    "@odata.type": "microsoft.graph.itemBody",
    "contentType": "String",
    "content": "Content value"
  },
  "completedDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone",
    "dateTime": "Date Time value",
    "timeZone": "Time Zone value"
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
    "@odata.type": "microsoft.graph.patternedRecurrence",
    "pattern": {
      "@odata.type": "microsoft.graph.recurrencePattern",
      "type": "String",
      "interval": 8,
      "month": 5,
      "dayOfMonth": 10,
      "daysOfWeek": [
        "String"
      ],
      "firstDayOfWeek": "String",
      "index": "String"
    },
    "range": {
      "@odata.type": "microsoft.graph.recurrenceRange",
      "type": "String",
      "startDate": "Date",
      "endDate": "Date",
      "recurrenceTimeZone": "Recurrence Time Zone value",
      "numberOfOccurrences": 3
    }
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
```

