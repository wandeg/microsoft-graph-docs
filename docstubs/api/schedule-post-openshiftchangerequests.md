---
title: "Add openShiftChangeRequests"
description: "Add openShiftChangeRequests by posting to the openShiftChangeRequests collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add openShiftChangeRequests

Namespace: microsoft.graph

Add openShiftChangeRequests by posting to the openShiftChangeRequests collection.

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
POST /me/joinedGroups/{groupId}/team/schedule/openShiftChangeRequests/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.

The following table shows the properties that are required when you create the [openShiftChangeRequest](../resources/openshiftchangerequest.md).

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
|openShiftId|String||



## Response
If successful, this method returns a `201 Created` response code and a [openShiftChangeRequest](../resources/openshiftchangerequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_openshiftchangerequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/openShiftChangeRequests
Content-type: application/json
Content-length: 468

{
  "@odata.type": "#microsoft.graph.openShiftChangeRequest",
  "assignedTo": "String",
  "state": "String",
  "senderMessage": "Sender Message value",
  "senderDateTime": "2016-12-31T23:57:59.5684903+00:00",
  "managerActionMessage": "Manager Action Message value",
  "managerActionDateTime": "2017-01-01T00:00:19.5432871+00:00",
  "senderUserId": "Sender User Id value",
  "managerUserId": "Manager User Id value",
  "openShiftId": "Open Shift Id value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openshiftchangerequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1013

{
  "@odata.type": "#microsoft.graph.openShiftChangeRequest",
  "id": "5e93a6d3-a6d3-5e93-d3a6-935ed3a6935e",
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
  "openShiftId": "Open Shift Id value"
}
```

