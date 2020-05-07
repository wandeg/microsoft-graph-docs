---
title: "bookingStaffMember resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# bookingStaffMember resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [bookingPerson](../resources/bookingperson.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|availabilityIsAffectedByPersonalCalendar|Boolean|**TODO: Add Description**|
|colorIndex|Int32|**TODO: Add Description**|
|displayName|String|**TODO: Add Description** Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|emailAddress|String|**TODO: Add Description** Inherited from [bookingPerson](../resources/bookingperson.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|role|bookingStaffRole|**TODO: Add Description**. Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.|
|useBusinessHours|Boolean|**TODO: Add Description**|
|workingHours|[bookingWorkHours](../resources/bookingworkhours.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "availabilityIsAffectedByPersonalCalendar": "Boolean",
  "colorIndex": "Integer",
  "role": "String",
  "useBusinessHours": "Boolean",
  "workingHours": [
    {
      "@odata.type": "microsoft.graph.bookingWorkHours"
    }
  ]
}
```

