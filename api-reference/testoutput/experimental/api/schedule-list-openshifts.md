---
title: "List openShifts"
description: "Get the openShifts from the openShifts navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List openShifts

Namespace: microsoft.graph

Get the openShifts from the openShifts navigation property.

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
GET /me/joinedGroups/{groupId}/team/schedule/openShifts
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [openShift](../resources/openshift.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_openshift"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/team/schedule/openShifts
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.openshift)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1346

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.openShift",
      "id": "91d9b661-b661-91d9-61b6-d99161b6d991",
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
      "sharedOpenShift": {
        "@odata.type": "microsoft.graph.openShiftItem",
        "startDateTime": "2016-12-31T23:59:24.7548426+03:00",
        "endDateTime": "2016-12-31T23:58:29.0720449+03:00",
        "theme": "String",
        "notes": "Notes value",
        "activities": [
          {
            "@odata.type": "microsoft.graph.shiftActivity",
            "isPaid": true,
            "code": "Code value"
          }
        ],
        "openSlotCount": 13
      },
      "draftOpenShift": {
        "@odata.type": "microsoft.graph.openShiftItem"
      },
      "schedulingGroupId": "Scheduling Group Id value"
    }
  ]
}
```

