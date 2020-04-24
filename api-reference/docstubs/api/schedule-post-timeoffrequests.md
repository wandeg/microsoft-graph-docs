---
title: "Create timeOffRequests"
description: "Create a new timeOffRequests object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create timeOffRequests

Namespace: microsoft.graph

Create a new timeOffRequests object.

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
POST /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/schedule/timeOffRequests
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [timeOffRequest](../resources/timeoffrequest.md) object.

The following table shows the properties that are required when you create the [timeOffRequest](../resources/timeoffrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|assignedTo|scheduleChangeRequestActor|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `sender`, `recipient`, `manager`, `system`, `unknownFutureValue`.|
|state|scheduleChangeState|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `pending`, `approved`, `declined`, `unknownFutureValue`.|
|senderMessage|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|managerActionMessage|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|managerActionDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderUserId|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|managerUserId|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|timeOffReasonId|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [timeOffRequest](../resources/timeoffrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_timeoffrequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/schedule/timeOffRequests
Content-Type: application/json
Content-length: 580

{
  "@odata.type": "#microsoft.graph.timeOffRequest",
  "assignedTo": "String",
  "state": "String",
  "senderMessage": "Sender Message value",
  "senderDateTime": "2017-01-01T00:00:08.189103+03:00",
  "managerActionMessage": "Manager Action Message value",
  "managerActionDateTime": "2017-01-01T00:03:04.8950901+03:00",
  "senderUserId": "Sender User Id value",
  "managerUserId": "Manager User Id value",
  "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
  "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
  "timeOffReasonId": "Time Off Reason Id value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeoffrequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.timeOffRequest",
  "id": "91811ffb-1ffb-9181-fb1f-8191fb1f8191",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "assignedTo": "String",
  "state": "String",
  "senderMessage": "Sender Message value",
  "senderDateTime": "2017-01-01T00:00:08.189103+03:00",
  "managerActionMessage": "Manager Action Message value",
  "managerActionDateTime": "2017-01-01T00:03:04.8950901+03:00",
  "senderUserId": "Sender User Id value",
  "managerUserId": "Manager User Id value",
  "startDateTime": "2017-01-01T00:02:03.6478792+03:00",
  "endDateTime": "2016-12-31T23:59:06.8319712+03:00",
  "timeOffReasonId": "Time Off Reason Id value"
}
```

