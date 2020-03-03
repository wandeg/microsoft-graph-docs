---
title: "Add staffMembers"
description: "Add staffMembers by posting to the staffMembers collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add staffMembers

Namespace: microsoft.graph

Add staffMembers by posting to the staffMembers collection.

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
POST /bookingBusinesses/{bookingBusinessesId}/staffMembers/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [bookingStaffMember](../resources/bookingstaffmember.md) object.

The following table shows the properties that are required when you create the [bookingStaffMember](../resources/bookingstaffmember.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String|Display name of this entity.
The display name is suitable for human-readable interfaces. Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|emailAddress|String|The e-mail address of this person. Inherited from [bookingPerson](../resources/bookingperson.md)|
|availabilityIsAffectedByPersonalCalendar|Boolean||
|colorIndex|Int32||
|role|Enumeration|. Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.|
|useBusinessHours|Boolean||
|workingHours|[bookingWorkHours](../resources/bookingworkhours.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_bookingstaffmember_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/bookingBusinesses/{bookingBusinessesId}/staffMembers
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
          "start": "12:02:01.9800000",
          "end": "12:02:50.7750000"
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
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingstaffmember"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 633

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
```

