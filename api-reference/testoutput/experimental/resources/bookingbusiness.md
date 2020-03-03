---
title: "bookingBusiness resource type"
description: "Represents a Microsot Bookings Business.
The bookingBusiness is the top level object which contains business information and related business objects such as appointments, customers, services and staff members."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# bookingBusiness resource type

Represents a Microsot Bookings Business.
The bookingBusiness is the top level object which contains business information and related business objects such as appointments, customers, services and staff members.


Inherits from [bookingNamedEntity](../resources/bookingNamedEntity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List bookingBusinesses](../api/bookingbusiness-list.md)|[bookingBusiness](../resources/bookingBusiness.md) collection|List properties and relationships of the [bookingBusiness](../resources/bookingbusiness.md) objects.|
|[Get bookingBusiness](../api/bookingbusiness-get.md)|[bookingBusiness](../resources/bookingBusiness.md)|Read properties and relationships of the [bookingBusiness](../resources/bookingbusiness.md) object.|
|[Create bookingBusiness](../api/bookingbusiness-post-bookingbusinesses.md)|[bookingBusiness](../resources/bookingBusiness.md)|Create a new [bookingBusiness](../resources/bookingbusiness.md) object.|
|[Delete bookingBusiness](../api/bookingbusiness-delete.md)|None|Deletes a [bookingBusiness](../resources/bookingbusiness.md).|
|[Update bookingBusiness](../api/bookingbusiness-update.md)|[bookingBusiness](../resources/bookingBusiness.md)|Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.|
|[List appointments](../api/bookingbusiness-list-appointments.md)|[bookingAppointment](../resources/bookingAppointment.md) collection|Get the bookingAppointments from the appointments navigation property.|
|[Add appointments](../api/bookingbusiness-post-appointments.md)|[bookingAppointment](../resources/bookingAppointment.md)|Add appointments by posting to the appointments collection.|
|[List calendarView](../api/bookingbusiness-list-calendarview.md)|[bookingAppointment](../resources/bookingAppointment.md) collection|Get the bookingAppointments from the calendarView navigation property.|
|[Add calendarView](../api/bookingbusiness-post-calendarview.md)|[bookingAppointment](../resources/bookingAppointment.md)|Add calendarView by posting to the calendarView collection.|
|[List customers](../api/bookingbusiness-list-customers.md)|[bookingCustomer](../resources/bookingCustomer.md) collection|Get the bookingCustomers from the customers navigation property.|
|[Add customers](../api/bookingbusiness-post-customers.md)|[bookingCustomer](../resources/bookingCustomer.md)|Add customers by posting to the customers collection.|
|[List services](../api/bookingbusiness-list-services.md)|[bookingService](../resources/bookingService.md) collection|Get the bookingServices from the services navigation property.|
|[Add services](../api/bookingbusiness-post-services.md)|[bookingService](../resources/bookingService.md)|Add services by posting to the services collection.|
|[List staffMembers](../api/bookingbusiness-list-staffmembers.md)|[bookingStaffMember](../resources/bookingStaffMember.md) collection|Get the bookingStaffMembers from the staffMembers navigation property.|
|[Add staffMembers](../api/bookingbusiness-post-staffmembers.md)|[bookingStaffMember](../resources/bookingStaffMember.md)|Add staffMembers by posting to the staffMembers collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[physicalAddress](../resources/physicalAddress.md)||
|businessHours|[bookingWorkHours](../resources/bookingWorkHours.md) collection||
|businessType|String||
|defaultCurrencyIso|String||
|displayName|String|Display name of this entity.
The display name is suitable for human-readable interfaces. Inherited from [bookingNamedEntity](../resources/bookingNamedEntity.md)|
|email|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isPublished|Boolean||
|phone|String||
|publicUrl|String||
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingSchedulingPolicy.md)||
|webSiteUrl|String|The URL of the business web site.
Example: https://www.contoso.com|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appointments|[bookingAppointment](../resources/bookingAppointment.md) collection|All appointments in this business.|
|calendarView|[bookingAppointment](../resources/bookingAppointment.md) collection|A calendar view of appointments in this business.|
|customers|[bookingCustomer](../resources/bookingCustomer.md) collection|All customers of this business.|
|services|[bookingService](../resources/bookingService.md) collection|All services offered by this business.|
|staffMembers|[bookingStaffMember](../resources/bookingStaffMember.md) collection|All staff members that provides services in this business.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingBusiness",
  "baseType": "microsoft.graph.bookingNamedEntity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingBusiness",
  "id": "String (identifier)",
  "displayName": "String",
  "businessType": "String",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress",
    "type": "String",
    "postOfficeBox": "String",
    "street": "String",
    "city": "String",
    "state": "String",
    "countryOrRegion": "String",
    "postalCode": "String"
  },
  "phone": "String",
  "email": "String",
  "webSiteUrl": "String",
  "defaultCurrencyIso": "String",
  "businessHours": [
    {
      "@odata.type": "microsoft.graph.bookingWorkHours"
    }
  ],
  "schedulingPolicy": {
    "@odata.type": "microsoft.graph.bookingSchedulingPolicy",
    "timeSlotInterval": "String (duration)",
    "minimumLeadTime": "String (duration)",
    "maximumAdvance": "String (duration)",
    "sendConfirmationsToOwner": true,
    "allowStaffSelection": true
  },
  "isPublished": true,
  "publicUrl": "String"
}
```

