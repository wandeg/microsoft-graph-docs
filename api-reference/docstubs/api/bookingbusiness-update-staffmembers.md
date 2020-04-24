---
title: "Update staffMembers"
description: "Update the properties of a staffMembers object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update staffMembers

Namespace: microsoft.graph

Update the properties of a staffMembers object.

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
PATCH /bookingBusinesses/{bookingBusinessesId}/staffMembers
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [bookingStaffMember](../resources/bookingstaffmember.md) object.

The following table shows the properties that are required when you create the [bookingStaffMember](../resources/bookingstaffmember.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|Display name of this entity.
The display name is suitable for human-readable interfaces. Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|emailAddress|String|The e-mail address of this person. Inherited from [bookingPerson](../resources/bookingperson.md)|
|availabilityIsAffectedByPersonalCalendar|Boolean|**TODO: Add Description**|
|colorIndex|Int32|**TODO: Add Description**|
|role|bookingStaffRole|**TODO: Add Description**. Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.|
|useBusinessHours|Boolean|**TODO: Add Description**|
|workingHours|[bookingWorkHours](../resources/bookingworkhours.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_staffmembers"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}/staffMembers
Content-Type: application/json
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
          "start": "12:02:33.8790000",
          "end": "12:02:09.0100000"
        }
      ]
    }
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
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
```

