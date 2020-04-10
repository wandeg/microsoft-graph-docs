---
title: "Update swapShiftsChangeRequest"
description: "Update the properties of a swapShiftsChangeRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update swapShiftsChangeRequest

Namespace: microsoft.graph

Update the properties of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.

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
PATCH /me/joinedGroups/{groupId}/team/schedule/swapShiftsChangeRequests/{swapShiftsChangeRequestId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.

The following table shows the properties that are required when you create the [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md).

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
|recipientActionMessage|String| Inherited from [offerShiftRequest](../resources/offershiftrequest.md)|
|recipientActionDateTime|DateTimeOffset| Inherited from [offerShiftRequest](../resources/offershiftrequest.md)|
|senderShiftId|String| Inherited from [offerShiftRequest](../resources/offershiftrequest.md)|
|recipientUserId|String| Inherited from [offerShiftRequest](../resources/offershiftrequest.md)|
|recipientShiftId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_swapshiftschangerequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/swapShiftsChangeRequests/{swapShiftsChangeRequestId}
Content-type: application/json
Content-length: 703

{
  "@odata.type": "#microsoft.graph.swapShiftsChangeRequest",
  "assignedTo": "String",
  "state": "String",
  "senderMessage": "Sender Message value",
  "senderDateTime": "2016-12-31T23:57:59.5684903+00:00",
  "managerActionMessage": "Manager Action Message value",
  "managerActionDateTime": "2017-01-01T00:00:19.5432871+00:00",
  "senderUserId": "Sender User Id value",
  "managerUserId": "Manager User Id value",
  "recipientActionMessage": "Recipient Action Message value",
  "recipientActionDateTime": "2016-12-31T23:57:49.4661232+00:00",
  "senderShiftId": "Sender Shift Id value",
  "recipientUserId": "Recipient User Id value",
  "recipientShiftId": "Recipient Shift Id value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1248

{
  "@odata.type": "#microsoft.graph.swapShiftsChangeRequest",
  "id": "3d4a7242-7242-3d4a-4272-4a3d42724a3d",
  "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
  "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
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
  "senderDateTime": "2016-12-31T23:57:59.5684903+00:00",
  "managerActionMessage": "Manager Action Message value",
  "managerActionDateTime": "2017-01-01T00:00:19.5432871+00:00",
  "senderUserId": "Sender User Id value",
  "managerUserId": "Manager User Id value",
  "recipientActionMessage": "Recipient Action Message value",
  "recipientActionDateTime": "2016-12-31T23:57:49.4661232+00:00",
  "senderShiftId": "Sender Shift Id value",
  "recipientUserId": "Recipient User Id value",
  "recipientShiftId": "Recipient Shift Id value"
}
```

