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
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [offerShiftRequest](../resources/offershiftrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_offershiftrequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/offerShiftRequests/{offerShiftRequestId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
    "id": "100554e9-54e9-1005-e954-0510e9540510",
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
    "recipientUserId": "Recipient User Id value"
  }
}
```

