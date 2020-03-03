---
title: "Create swapShiftsChangeRequest"
description: "Create a new swapShiftsChangeRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create swapShiftsChangeRequest

Namespace: microsoft.graph

Create a new [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.

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
POST /me/joinedGroups/{groupId}/team/schedule/swapShiftsChangeRequests
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
POST https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/team/schedule/swapShiftsChangeRequests
Content-type: application/json
Content-length: 703

{
  "@odata.type": "#microsoft.graph.swapShiftsChangeRequest",
  "assignedTo": "String",
  "state": "String",
  "senderMessage": "Sender Message value",
  "senderDateTime": "2016-12-31T23:59:47.8447466+03:00",
  "managerActionMessage": "Manager Action Message value",
  "managerActionDateTime": "2017-01-01T00:03:26.1696907+03:00",
  "senderUserId": "Sender User Id value",
  "managerUserId": "Manager User Id value",
  "recipientActionMessage": "Recipient Action Message value",
  "recipientActionDateTime": "2016-12-31T23:58:22.0066573+03:00",
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
Content-Length: 1247

{
  "@odata.type": "#microsoft.graph.swapShiftsChangeRequest",
  "id": "4e13d3d1-d3d1-4e13-d1d3-134ed1d3134e",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
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
  "senderDateTime": "2016-12-31T23:59:47.8447466+03:00",
  "managerActionMessage": "Manager Action Message value",
  "managerActionDateTime": "2017-01-01T00:03:26.1696907+03:00",
  "senderUserId": "Sender User Id value",
  "managerUserId": "Manager User Id value",
  "recipientActionMessage": "Recipient Action Message value",
  "recipientActionDateTime": "2016-12-31T23:58:22.0066573+03:00",
  "senderShiftId": "Sender Shift Id value",
  "recipientUserId": "Recipient User Id value",
  "recipientShiftId": "Recipient Shift Id value"
}
```

