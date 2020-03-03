---
title: "bookingStaffMember resource type"
description: "Represents a staff member who provides services in a business."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# bookingStaffMember resource type


Namespace: microsoft.graph

Represents a staff member who provides services in a business.


Inherits from [bookingPerson](../resources/bookingperson.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List bookingStaffMembers](../api/bookingstaffmember-list.md)|[bookingStaffMember](../resources/bookingstaffmember.md) collection|List properties and relationships of the [bookingStaffMember](../resources/bookingstaffmember.md) objects.|
|[Get bookingStaffMember](../api/bookingstaffmember-get.md)|[bookingStaffMember](../resources/bookingstaffmember.md)|Read properties and relationships of the [bookingStaffMember](../resources/bookingstaffmember.md) object.|
|[Create bookingStaffMember](../api/bookingstaffmember-create.md)|[bookingStaffMember](../resources/bookingstaffmember.md)|Create a new [bookingStaffMember](../resources/bookingstaffmember.md) object.|
|[Delete bookingStaffMember](../api/bookingstaffmember-delete.md)|None|Deletes a [bookingStaffMember](../resources/bookingstaffmember.md).|
|[Update bookingStaffMember](../api/bookingstaffmember-update.md)|[bookingStaffMember](../resources/bookingstaffmember.md)|Update the properties of a [bookingStaffMember](../resources/bookingstaffmember.md) object.|
|[List staffMembers](../api/bookingbusiness-list-staffmembers.md)|[bookingStaffMember](../resources/bookingstaffmember.md) collection|Get the bookingStaffMembers from the staffMembers navigation property.|
|[Add staffMembers](../api/bookingbusiness-post-staffmembers.md)|[bookingStaffMember](../resources/bookingstaffmember.md)|Add staffMembers by posting to the staffMembers collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|availabilityIsAffectedByPersonalCalendar|Boolean||
|colorIndex|Int32||
|displayName|String|Display name of this entity.
The display name is suitable for human-readable interfaces. Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|emailAddress|String|The e-mail address of this person. Inherited from [bookingPerson](../resources/bookingperson.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|role|Enumeration|. Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.|
|useBusinessHours|Boolean||
|workingHours|[bookingWorkHours](../resources/bookingworkhours.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingStaffMember",
  "baseType": "microsoft.graph.bookingPerson",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingStaffMember",
  "id": "String (identifier)",
  "displayName": "String",
  "emailAddress": "String",
  "availabilityIsAffectedByPersonalCalendar": true,
  "colorIndex": 1024,
  "role": "String",
  "useBusinessHours": true,
  "workingHours": [
    {
      "@odata.type": "microsoft.graph.bookingWorkHours"
    }
  ]
}
```

