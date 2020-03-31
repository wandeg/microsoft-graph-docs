---
title: "Update bookingStaffMember"
description: "Update the properties of a bookingStaffMember object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update bookingStaffMember

Namespace: microsoft.graph

Update the properties of a [bookingStaffMember](../resources/bookingstaffmember.md) object.

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
PATCH /bookingBusinesses/{bookingBusinessesId}/staffMembers/{bookingStaffMemberId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [bookingStaffMember](../resources/bookingstaffmember.md) object.

The following table shows the properties that are required when you create the [bookingStaffMember](../resources/bookingstaffmember.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|emailAddress|String| Inherited from [bookingPerson](../resources/bookingperson.md)|
|availabilityIsAffectedByPersonalCalendar|Boolean||
|colorIndex|Int32||
|role|Enumeration| Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.|
|useBusinessHours|Boolean||
|workingHours|[bookingWorkHours](../resources/bookingworkhours.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_bookingstaffmember"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}/staffMembers/{bookingStaffMemberId}
Content-type: application/json
Content-length: 584

{
  "@odata.type": "#microsoft.graph.bookingStaffMember",
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
          "start": "11:59:31.2520000",
          "end": "11:56:43.2870000"
        }
      ]
    }
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 633

{
  "@odata.type": "#microsoft.graph.bookingStaffMember",
  "id": "4125d550-d550-4125-50d5-254150d52541",
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
          "start": "11:59:31.2520000",
          "end": "11:56:43.2870000"
        }
      ]
    }
  ]
}
```

