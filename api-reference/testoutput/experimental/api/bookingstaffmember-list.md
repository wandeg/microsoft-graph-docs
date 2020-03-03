---
title: "List bookingStaffMembers"
description: "List properties and relationships of the bookingStaffMember objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List bookingStaffMembers

Namespace: microsoft.graph

List properties and relationships of the [bookingStaffMember](../resources/bookingstaffmember.md) objects.

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
GET /bookingBusinesses/{bookingBusinessesId}/staffMembers
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_bookingstaffmember"
}
-->
``` http
GET https://graph.microsoft.com/localtest/bookingBusinesses/{bookingBusinessesId}/staffMembers
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.bookingstaffmember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 750

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bookingStaffMember",
      "id": "ff3e1fa8-1fa8-ff3e-a81f-3effa81f3eff",
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
              "start": "12:02:01.9800000",
              "end": "12:02:50.7750000"
            }
          ]
        }
      ]
    }
  ]
}
```

