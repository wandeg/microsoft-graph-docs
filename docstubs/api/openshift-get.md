---
title: "Get openShift"
description: "Read properties and relationships of the openShift object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get openShift

Namespace: microsoft.graph

Read properties and relationships of the [openShift](../resources/openshift.md) object.

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
GET /me/joinedGroups/{groupId}/team/schedule/openShifts/{openShiftId}
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
If successful, this method returns a `200 OK` response code and [openShift](../resources/openshift.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_openshift"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/team/schedule/openShifts/{openShiftId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.openShift"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1259

{
  "value": {
    "@odata.type": "#microsoft.graph.openShift",
    "id": "0d9ec7e1-c7e1-0d9e-e1c7-9e0de1c79e0d",
    "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
    "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
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
      "startDateTime": "2017-01-01T00:02:37.6086584+03:00",
      "endDateTime": "2016-12-31T23:57:47.3167027+03:00",
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
}
```

