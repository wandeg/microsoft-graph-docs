---
title: "List timeOffRequests"
description: "Get the timeOffRequests from the timeOffRequests navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List timeOffRequests

Namespace: microsoft.graph

Get the timeOffRequests from the timeOffRequests navigation property.

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
GET /me/joinedGroups/{groupId}/team/schedule/timeOffRequests
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
If successful, this method returns a `200 OK` response code and a collection of [timeOffRequest](../resources/timeoffrequest.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/timeOffRequests
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.timeoffrequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1275

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.timeOffRequest",
      "id": "f5a642e1-42e1-f5a6-e142-a6f5e142a6f5",
      "createdDateTime": "2017-01-01T00:01:44.2536508+00:00",
      "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00",
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
      "senderDateTime": "2016-12-31T23:56:47.1140844+00:00",
      "managerActionMessage": "Manager Action Message value",
      "managerActionDateTime": "2017-01-01T00:01:28.2211043+00:00",
      "senderUserId": "Sender User Id value",
      "managerUserId": "Manager User Id value",
      "startDateTime": "2016-12-31T23:57:02.6825424+00:00",
      "endDateTime": "2016-12-31T23:59:12.2321935+00:00",
      "timeOffReasonId": "Time Off Reason Id value"
    }
  ]
}
```

