---
title: "List timeOffRequests"
description: "Get the timeOffRequests from the timeOffRequests navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List timeOffRequests

Namespace: microsoft.graph

Get the timeOffRequests from the timeOffRequests navigation property.

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
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/schedule/timeOffRequests
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [timeOffRequest](../resources/timeoffrequest.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/schedule/timeOffRequests
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.timeoffrequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```

