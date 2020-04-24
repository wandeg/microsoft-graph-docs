---
title: "bookingStaffMember resource type"
description: "Represents a staff member who provides services in a business."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# bookingStaffMember resource type


Namespace: microsoft.graph

Represents a staff member who provides services in a business.


Inherits from [bookingPerson](../resources/bookingperson.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get bookingStaffMember](../api/bookingstaffmember-get.md)|[bookingStaffMember](../resources/bookingstaffmember.md)|Read the properties and relationships of a [bookingStaffMember](../resources/bookingstaffmember.md) object.|
|[Update bookingStaffMember](../api/bookingstaffmember-update.md)|[bookingStaffMember](../resources/bookingstaffmember.md)|Update the properties of a [bookingStaffMember](../resources/bookingstaffmember.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|availabilityIsAffectedByPersonalCalendar|Boolean|**TODO: Add Description**|
|colorIndex|Int32|**TODO: Add Description**|
|displayName|String|Display name of this entity.
The display name is suitable for human-readable interfaces. Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|emailAddress|String|The e-mail address of this person. Inherited from [bookingPerson](../resources/bookingperson.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|role|bookingStaffRole|**TODO: Add Description**. Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.|
|useBusinessHours|Boolean|**TODO: Add Description**|
|workingHours|[bookingWorkHours](../resources/bookingworkhours.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

