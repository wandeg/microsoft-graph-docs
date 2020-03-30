---
title: "Get bookingStaffMember"
description: "Read properties and relationships of the bookingStaffMember object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get bookingStaffMember

Namespace: microsoft.graph

Read properties and relationships of the [bookingStaffMember](../resources/bookingstaffmember.md) object.

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
GET /bookingBusinesses/{bookingBusinessesId}/staffMembers/{bookingStaffMemberId}
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
If successful, this method returns a `200 OK` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_bookingstaffmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}/staffMembers/{bookingStaffMemberId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 694

{
  "value": {
    "@odata.type": "#microsoft.graph.bookingStaffMember",
    "id": "3e3da994-a994-3e3d-94a9-3d3e94a93d3e",
    "displayName": "Display Name value",
    "emailAddress": "Email Address value",
    "availabilityIsAffectedByPersonalCalendar": true,
    "colorIndex": 10,
    "role": "String",
    "useBusinessHours": true,
    "workingHours": [
      {
        "@odata.type": "microsoft.graph.bookingWorkHours",
        "day": "String",
        "timeSlots": [
          {
            "@odata.type": "microsoft.graph.bookingWorkTimeSlot",
            "start": "11:58:13.3440000",
            "end": "12:01:29.0340000"
          }
        ]
      }
    ]
  }
}
```

