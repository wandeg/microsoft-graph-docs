---
title: "Update timeOffRequest"
description: "Update the properties of a timeOffRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update timeOffRequest

Namespace: microsoft.graph

Update the properties of a [timeOffRequest](../resources/timeoffrequest.md) object.

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
PATCH /me/joinedGroups/{groupId}/team/schedule/timeOffRequests/{timeOffRequestId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [timeOffRequest](../resources/timeoffrequest.md) object.

The following table shows the properties that are required when you create the [timeOffRequest](../resources/timeoffrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|assignedTo|Enumeration| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `sender`, `recipient`, `manager`, `system`, `unknownFutureValue`.|
|state|Enumeration| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `pending`, `approved`, `declined`, `unknownFutureValue`.|
|senderMessage|String| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderDateTime|DateTimeOffset| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|managerActionMessage|String| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|managerActionDateTime|DateTimeOffset| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderUserId|String| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|managerUserId|String| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|startDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||
|timeOffReasonId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [timeOffRequest](../resources/timeoffrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_timeoffrequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/timeOffRequests/{timeOffRequestId}
Content-type: application/json
Content-length: 580

{
  "@odata.type": "#microsoft.graph.timeOffRequest",
  "assignedTo": "String",
  "state": "String",
  "senderMessage": "Sender Message value",
  "senderDateTime": "2016-12-31T23:56:45.3116094+03:00",
  "managerActionMessage": "Manager Action Message value",
  "managerActionDateTime": "2016-12-31T23:59:22.119248+03:00",
  "senderUserId": "Sender User Id value",
  "managerUserId": "Manager User Id value",
  "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
  "endDateTime": "2017-01-01T00:01:45.7287553+03:00",
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
Content-Length: 1125

{
  "@odata.type": "#microsoft.graph.timeOffRequest",
  "id": "9db3163d-163d-9db3-3d16-b39d3d16b39d",
  "createdDateTime": "2017-01-01T00:01:00.9969079+03:00",
  "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00",
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
  "senderDateTime": "2016-12-31T23:56:45.3116094+03:00",
  "managerActionMessage": "Manager Action Message value",
  "managerActionDateTime": "2016-12-31T23:59:22.119248+03:00",
  "senderUserId": "Sender User Id value",
  "managerUserId": "Manager User Id value",
  "startDateTime": "2017-01-01T00:03:15.8315541+03:00",
  "endDateTime": "2017-01-01T00:01:45.7287553+03:00",
  "timeOffReasonId": "Time Off Reason Id value"
}
```

