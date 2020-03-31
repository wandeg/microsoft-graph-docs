---
title: "List shifts"
description: "Get the shifts from the shifts navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List shifts

Namespace: microsoft.graph

Get the shifts from the shifts navigation property.

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
GET /me/joinedGroups/{groupId}/team/schedule/shifts
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
If successful, this method returns a `200 OK` response code and a collection of [shift](../resources/shift.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_shift"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/shifts
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.shift)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1330

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.shift",
      "id": "e1619457-9457-e161-5794-61e1579461e1",
      "createdDateTime": "2017-01-01T00:01:55.391884+03:00",
      "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
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
        "startDateTime": "2016-12-31T23:57:07.1037922+03:00",
        "endDateTime": "2016-12-31T23:57:36.8091086+03:00",
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
  ]
}
```

