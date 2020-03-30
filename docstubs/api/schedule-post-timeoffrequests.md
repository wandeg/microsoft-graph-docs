---
title: "Add timeOffRequests"
description: "Add timeOffRequests by posting to the timeOffRequests collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add timeOffRequests

Namespace: microsoft.graph

Add timeOffRequests by posting to the timeOffRequests collection.

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
POST /me/joinedGroups/{groupId}/team/schedule/timeOffRequests/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [timeOffRequest](../resources/timeoffrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_timeoffrequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/timeOffRequests
Content-type: application/json
Content-length: 581

{
  "@odata.type": "#microsoft.graph.timeOffRequest",
  "assignedTo": "String",
  "state": "String",
  "senderMessage": "Sender Message value",
  "senderDateTime": "2016-12-31T23:56:33.1925831+03:00",
  "managerActionMessage": "Manager Action Message value",
  "managerActionDateTime": "2016-12-31T23:58:11.6415176+03:00",
  "senderUserId": "Sender User Id value",
  "managerUserId": "Manager User Id value",
  "startDateTime": "2017-01-01T00:02:37.6086584+03:00",
  "endDateTime": "2016-12-31T23:57:47.3167027+03:00",
  "timeOffReasonId": "Time Off Reason Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeoffrequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1126

{
  "@odata.type": "#microsoft.graph.timeOffRequest",
  "id": "e256eefe-eefe-e256-feee-56e2feee56e2",
  "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
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
  "senderDateTime": "2016-12-31T23:56:33.1925831+03:00",
  "managerActionMessage": "Manager Action Message value",
  "managerActionDateTime": "2016-12-31T23:58:11.6415176+03:00",
  "senderUserId": "Sender User Id value",
  "managerUserId": "Manager User Id value",
  "startDateTime": "2017-01-01T00:02:37.6086584+03:00",
  "endDateTime": "2016-12-31T23:57:47.3167027+03:00",
  "timeOffReasonId": "Time Off Reason Id value"
}
```

