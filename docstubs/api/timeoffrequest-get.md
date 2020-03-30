---
title: "Get timeOffRequest"
description: "Read properties and relationships of the timeOffRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get timeOffRequest

Namespace: microsoft.graph

Read properties and relationships of the [timeOffRequest](../resources/timeoffrequest.md) object.

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
GET /me/joinedGroups/{groupId}/team/schedule/timeOffRequests/{timeOffRequestId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [timeOffRequest](../resources/timeoffrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/timeOffRequests/{timeOffRequestId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1203

{
  "value": {
    "@odata.type": "#microsoft.graph.timeOffRequest",
    "id": "9342b9d7-b9d7-9342-d7b9-4293d7b94293",
    "createdDateTime": "2016-12-31T23:56:52.9286964+00:00",
    "lastModifiedDateTime": "2017-01-01T00:02:50.3839766+00:00",
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
    "senderDateTime": "2017-01-01T00:03:30.8490132+00:00",
    "managerActionMessage": "Manager Action Message value",
    "managerActionDateTime": "2017-01-01T00:02:25.4934169+00:00",
    "senderUserId": "Sender User Id value",
    "managerUserId": "Manager User Id value",
    "startDateTime": "2016-12-31T23:58:12.4547779+00:00",
    "endDateTime": "2016-12-31T23:56:38.1219845+00:00",
    "timeOffReasonId": "Time Off Reason Id value"
  }
}
```

