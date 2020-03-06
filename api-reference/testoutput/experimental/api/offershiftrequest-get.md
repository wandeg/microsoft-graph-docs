---
title: "Get offerShiftRequest"
description: "Read properties and relationships of the offerShiftRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get offerShiftRequest

Namespace: microsoft.graph

Read properties and relationships of the [offerShiftRequest](../resources/offershiftrequest.md) object.

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
GET /me/joinedGroups/{groupId}/team/schedule/offerShiftRequests/{offerShiftRequestId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/team/schedule/offerShiftRequests/{offerShiftRequestId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.offerShiftRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1270

{
  "value": {
    "@odata.type": "#microsoft.graph.offerShiftRequest",
    "id": "d6a7392d-392d-d6a7-2d39-a7d62d39a7d6",
    "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
    "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00",
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
    "senderDateTime": "2017-01-01T00:00:50.3002047+03:00",
    "managerActionMessage": "Manager Action Message value",
    "managerActionDateTime": "2016-12-31T23:58:00.9521432+03:00",
    "senderUserId": "Sender User Id value",
    "managerUserId": "Manager User Id value",
    "recipientActionMessage": "Recipient Action Message value",
    "recipientActionDateTime": "2017-01-01T00:01:59.9496671+03:00",
    "senderShiftId": "Sender Shift Id value",
    "recipientUserId": "Recipient User Id value"
  }
}
```

