---
title: "List staffMembers"
description: "Get the bookingStaffMembers from the staffMembers navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List staffMembers

Get the bookingStaffMembers from the staffMembers navigation property.

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
GET https://graph.microsoft.com/docs\api/bookingBusinesses/{bookingBusinessesId}/staffMembers
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
      "id": "b8869257-9257-b886-5792-86b8579286b8",
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
              "start": "11:59:43.5410000",
              "end": "12:01:36.3070000"
            }
          ]
        }
      ]
    }
  ]
}
```

