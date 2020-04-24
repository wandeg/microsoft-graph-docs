---
title: "List staffMembers"
description: "Get the bookingStaffMembers from the staffMembers navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List staffMembers

Namespace: microsoft.graph

Get the bookingStaffMembers from the staffMembers navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

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
|Authorization|Bearer {token}. Required|

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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.bookingstaffmember)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bookingStaffMember",
      "id": "a7b759a7-59a7-a7b7-a759-b7a7a759b7a7",
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
              "start": "12:02:33.8790000",
              "end": "12:02:09.0100000"
            }
          ]
        }
      ]
    }
  ]
}
```

