---
title: "List openShiftChangeRequests"
description: "List properties and relationships of the openShiftChangeRequest objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List openShiftChangeRequests

Namespace: microsoft.graph

List properties and relationships of the [openShiftChangeRequest](../resources/openshiftchangerequest.md) objects.

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
GET /me/joinedGroups/{groupId}/team/schedule/openShiftChangeRequests
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [openShiftChangeRequest](../resources/openshiftchangerequest.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_openshiftchangerequest"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/team/schedule/openShiftChangeRequests
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.openshiftchangerequest)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1153

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.openShiftChangeRequest",
      "id": "e4d2a3c0-a3c0-e4d2-c0a3-d2e4c0a3d2e4",
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
      "openShiftId": "Open Shift Id value"
    }
  ]
}
```

