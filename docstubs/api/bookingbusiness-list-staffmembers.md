---
title: "List staffMembers"
description: "Get the bookingStaffMembers from the staffMembers navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List staffMembers

Namespace: microsoft.graph

Get the bookingStaffMembers from the staffMembers navigation property.

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
GET /bookingBusinesses/{bookingBusinessesId}/staffMembers
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
If successful, this method returns a `200 OK` response code and a collection of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_bookingstaffmember"
}
-->
``` http
GET https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}/staffMembers
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
      "id": "9843175d-175d-9843-5d17-43985d174398",
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
              "start": "11:56:56.0110000",
              "end": "11:57:00.7790000"
            }
          ]
        }
      ]
    }
  ]
}
```

