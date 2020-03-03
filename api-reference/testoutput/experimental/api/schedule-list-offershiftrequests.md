---
title: "List offerShiftRequests"
description: "Get the offerShiftRequests from the offerShiftRequests navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List offerShiftRequests

Get the offerShiftRequests from the offerShiftRequests navigation property.

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
GET /me/joinedGroups/{groupId}/team/schedule/offerShiftRequests
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [offerShiftRequest](../resources/offershiftrequest.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/me/joinedGroups/{groupId}/team/schedule/offerShiftRequests
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.offershiftrequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1344

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.offerShiftRequest",
      "id": "55744b00-4b00-5574-004b-7455004b7455",
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
      "recipientUserId": "Recipient User Id value"
    }
  ]
}
```

