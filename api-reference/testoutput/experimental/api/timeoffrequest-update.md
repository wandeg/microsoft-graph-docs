---
title: "Update timeOffRequest"
description: "Update the properties of a timeOffRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update timeOffRequest

Update the properties of a [timeOffRequest](../resources/timeoffrequest.md) object.

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
PATCH /me/joinedGroups/{groupId}/team/schedule/timeOffRequests/{timeOffRequestId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [timeOffRequest](../resources/timeOffRequest.md) object.

The following table shows the properties that are required when you create the [timeOffRequest](../resources/timeoffrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|assignedTo|Enumeration| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md). Possible values are: `sender`, `recipient`, `manager`, `system`, `unknownFutureValue`.|
|state|Enumeration| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md). Possible values are: `pending`, `approved`, `declined`, `unknownFutureValue`.|
|senderMessage|String| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md)|
|senderDateTime|DateTimeOffset| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md)|
|managerActionMessage|String| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md)|
|managerActionDateTime|DateTimeOffset| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md)|
|senderUserId|String| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md)|
|managerUserId|String| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md)|
|startDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||
|timeOffReasonId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [timeOffRequest](../resources/timeoffrequest.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_timeoffrequest"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/me/joinedGroups/{groupId}/team/schedule/timeOffRequests/{timeOffRequestId}
Content-type: application/json
Content-length: 581

{
  "@odata.type": "#microsoft.graph.timeOffRequest",
  "assignedTo": "String",
  "state": "String",
  "senderMessage": "Sender Message value",
  "senderDateTime": "2016-12-31T23:58:57.5545713+03:00",
  "managerActionMessage": "Manager Action Message value",
  "managerActionDateTime": "2016-12-31T23:58:19.3888566+03:00",
  "senderUserId": "Sender User Id value",
  "managerUserId": "Manager User Id value",
  "startDateTime": "2017-01-01T00:03:15.6077862+03:00",
  "endDateTime": "2017-01-01T00:01:17.3856072+03:00",
  "timeOffReasonId": "Time Off Reason Id value"
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
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.timeOffRequest",
  "id": "2ecb49a3-49a3-2ecb-a349-cb2ea349cb2e",
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
  "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00",
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
  "senderDateTime": "2016-12-31T23:58:57.5545713+03:00",
  "managerActionMessage": "Manager Action Message value",
  "managerActionDateTime": "2016-12-31T23:58:19.3888566+03:00",
  "senderUserId": "Sender User Id value",
  "managerUserId": "Manager User Id value",
  "startDateTime": "2017-01-01T00:03:15.6077862+03:00",
  "endDateTime": "2017-01-01T00:01:17.3856072+03:00",
  "timeOffReasonId": "Time Off Reason Id value"
}
```

