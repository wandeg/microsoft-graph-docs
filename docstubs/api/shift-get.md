---
title: "Get shift"
description: "Read properties and relationships of the shift object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get shift

Namespace: microsoft.graph

Read properties and relationships of the [shift](../resources/shift.md) object.

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
GET /me/joinedGroups/{groupId}/team/schedule/shifts/{shiftId}
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
If successful, this method returns a `200 OK` response code and [shift](../resources/shift.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_shift"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/shifts/{shiftId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1243

{
  "value": {
    "@odata.type": "#microsoft.graph.shift",
    "id": "5c6ac5d4-c5d4-5c6a-d4c5-6a5cd4c56a5c",
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
    "sharedShift": {
      "@odata.type": "microsoft.graph.shiftItem",
      "startDateTime": "2016-12-31T23:58:12.4547779+00:00",
      "endDateTime": "2016-12-31T23:56:38.1219845+00:00",
      "theme": "String",
      "notes": "Notes value",
      "activities": [
        {
          "@odata.type": "microsoft.graph.shiftActivity",
          "isPaid": true,
          "code": "Code value"
        }
      ]
    },
    "draftShift": {
      "@odata.type": "microsoft.graph.shiftItem"
    },
    "userId": "User Id value",
    "schedulingGroupId": "Scheduling Group Id value"
  }
}
```

