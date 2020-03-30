---
title: "Update offerShiftRequest"
description: "Update the properties of a offerShiftRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update offerShiftRequest

Namespace: microsoft.graph

Update the properties of a [offerShiftRequest](../resources/offershiftrequest.md) object.

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
PATCH /me/joinedGroups/{groupId}/team/schedule/offerShiftRequests/{offerShiftRequestId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [offerShiftRequest](../resources/offershiftrequest.md) object.

The following table shows the properties that are required when you create the [offerShiftRequest](../resources/offershiftrequest.md).

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
|recipientActionMessage|String||
|recipientActionDateTime|DateTimeOffset||
|senderShiftId|String||
|recipientUserId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_offershiftrequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/offerShiftRequests/{offerShiftRequestId}
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.offerShiftRequest",
  "assignedTo": "String",
  "state": "String",
  "senderMessage": "Sender Message value",
  "senderDateTime": "2016-12-31T23:57:58.214123+03:00",
  "managerActionMessage": "Manager Action Message value",
  "managerActionDateTime": "2016-12-31T23:57:47.3559085+03:00",
  "senderUserId": "Sender User Id value",
  "managerUserId": "Manager User Id value",
  "recipientActionMessage": "Recipient Action Message value",
  "recipientActionDateTime": "2017-01-01T00:01:29.2454102+03:00",
  "senderShiftId": "Sender Shift Id value",
  "recipientUserId": "Recipient User Id value"
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
Content-Length: 1190

{
  "@odata.type": "#microsoft.graph.offerShiftRequest",
  "id": "af3d44bd-44bd-af3d-bd44-3dafbd443daf",
  "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
  "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
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
  "senderDateTime": "2016-12-31T23:57:58.214123+03:00",
  "managerActionMessage": "Manager Action Message value",
  "managerActionDateTime": "2016-12-31T23:57:47.3559085+03:00",
  "senderUserId": "Sender User Id value",
  "managerUserId": "Manager User Id value",
  "recipientActionMessage": "Recipient Action Message value",
  "recipientActionDateTime": "2017-01-01T00:01:29.2454102+03:00",
  "senderShiftId": "Sender Shift Id value",
  "recipientUserId": "Recipient User Id value"
}
```

