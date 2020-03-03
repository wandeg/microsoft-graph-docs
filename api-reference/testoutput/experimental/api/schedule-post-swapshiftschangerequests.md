---
title: "Add swapShiftsChangeRequests"
description: "Add swapShiftsChangeRequests by posting to the swapShiftsChangeRequests collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add swapShiftsChangeRequests

Add swapShiftsChangeRequests by posting to the swapShiftsChangeRequests collection.

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
POST /me/joinedGroups/{groupId}/team/schedule/swapShiftsChangeRequests/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the swapShiftsChangeRequest object.

The following table shows the properties that are required when you create the swapShiftsChangeRequest.

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
|recipientActionMessage|String| Inherited from [offerShiftRequest](../resources/offerShiftRequest.md)|
|recipientActionDateTime|DateTimeOffset| Inherited from [offerShiftRequest](../resources/offerShiftRequest.md)|
|senderShiftId|String| Inherited from [offerShiftRequest](../resources/offerShiftRequest.md)|
|recipientUserId|String| Inherited from [offerShiftRequest](../resources/offerShiftRequest.md)|
|recipientShiftId|String||



## Response
If successful, this method returns a `201 Created` response code and a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_swapshiftschangerequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/me/joinedGroups/{groupId}/team/schedule/swapShiftsChangeRequests
Content-type: application/json
Content-length: 703

{
  "@odata.type": "#microsoft.graph.swapShiftsChangeRequest",
  "assignedTo": "String",
  "state": "String",
  "senderMessage": "Sender Message value",
  "senderDateTime": "2016-12-31T23:58:57.5545713+03:00",
  "managerActionMessage": "Manager Action Message value",
  "managerActionDateTime": "2016-12-31T23:58:19.3888566+03:00",
  "senderUserId": "Sender User Id value",
  "managerUserId": "Manager User Id value",
  "recipientActionMessage": "Recipient Action Message value",
  "recipientActionDateTime": "2016-12-31T23:59:57.9878243+03:00",
  "senderShiftId": "Sender Shift Id value",
  "recipientUserId": "Recipient User Id value",
  "recipientShiftId": "Recipient Shift Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.swapshiftschangerequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1248

{
  "@odata.type": "#microsoft.graph.swapShiftsChangeRequest",
  "id": "ebc81efb-1efb-ebc8-fb1e-c8ebfb1ec8eb",
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
  "recipientActionMessage": "Recipient Action Message value",
  "recipientActionDateTime": "2016-12-31T23:59:57.9878243+03:00",
  "senderShiftId": "Sender Shift Id value",
  "recipientUserId": "Recipient User Id value",
  "recipientShiftId": "Recipient Shift Id value"
}
```

