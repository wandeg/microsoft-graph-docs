---
title: "bookingBusiness resource type"
description: "Represents a Microsot Bookings Business.
The bookingBusiness is the top level object which contains business information and related business objects such as appointments, customers, services and staff members."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# bookingBusiness resource type


Namespace: microsoft.graph

Represents a Microsot Bookings Business.
The bookingBusiness is the top level object which contains business information and related business objects such as appointments, customers, services and staff members.


Inherits from [bookingNamedEntity](../resources/bookingnamedentity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List bookingBusinesses](../api/bookingbusiness-list.md)|[bookingBusiness](../resources/bookingbusiness.md) collection|Get a list of the [bookingBusiness](../resources/bookingbusiness.md) objects and their properties.|
|[Get bookingBusiness](../api/bookingbusiness-get.md)|[bookingBusiness](../resources/bookingbusiness.md)|Read the properties and relationships of a [bookingBusiness](../resources/bookingbusiness.md) object.|
|[Create bookingBusiness](../api/bookingbusiness-post-bookingbusinesses.md)|[bookingBusiness](../resources/bookingbusiness.md)|Create a new [bookingBusiness](../resources/bookingbusiness.md) object.|
|[Delete bookingBusiness](../api/bookingbusiness-delete.md)|None|Deletes a [bookingBusiness](../resources/bookingbusiness.md) object.|
|[Update bookingBusiness](../api/bookingbusiness-update.md)|[bookingBusiness](../resources/bookingbusiness.md)|Update the properties of a [bookingBusiness](../resources/bookingbusiness.md) object.|
|[publish](../api/bookingbusiness-publish.md)|None|**TODO: Add Description**|
|[unpublish](../api/bookingbusiness-unpublish.md)|None|**TODO: Add Description**|
|[List appointments](../api/bookingbusiness-list-appointments.md)|[bookingAppointment](../resources/bookingappointment.md) collection|Get the bookingAppointments from the appointments navigation property.|
|[Create appointments](../api/bookingbusiness-post-appointments.md)|[bookingAppointment](../resources/bookingappointment.md)|Create a new appointments object.|
|[Delete appointments](../api/bookingbusiness-delete-appointments.md)|None|Delete an [bookingAppointment](../resources/bookingappointment.md) object.|
|[Update appointments](../api/bookingbusiness-update-appointments.md)|[bookingAppointment](../resources/bookingappointment.md)|Update the properties of an appointments object.|
|[Get bookingAppointment](../api/bookingappointment-get.md)|[bookingAppointment](../resources/bookingappointment.md)|Read the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object.|
|[List calendarView](../api/bookingbusiness-list-calendarview.md)|[bookingAppointment](../resources/bookingappointment.md) collection|Get the bookingAppointments from the calendarView navigation property.|
|[Create calendarView](../api/bookingbusiness-post-calendarview.md)|[bookingAppointment](../resources/bookingappointment.md)|Create a new calendarView object.|
|[Delete calendarView](../api/bookingbusiness-delete-calendarview.md)|None|Delete a [bookingAppointment](../resources/bookingappointment.md) object.|
|[Update calendarView](../api/bookingbusiness-update-calendarview.md)|[bookingAppointment](../resources/bookingappointment.md)|Update the properties of a calendarView object.|
|[Get bookingAppointment](../api/bookingappointment-get.md)|[bookingAppointment](../resources/bookingappointment.md)|Read the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object.|
|[List customers](../api/bookingbusiness-list-customers.md)|[bookingCustomer](../resources/bookingcustomer.md) collection|Get the bookingCustomers from the customers navigation property.|
|[Create customers](../api/bookingbusiness-post-customers.md)|[bookingCustomer](../resources/bookingcustomer.md)|Create a new customers object.|
|[Delete customers](../api/bookingbusiness-delete-customers.md)|None|Delete a [bookingCustomer](../resources/bookingcustomer.md) object.|
|[Update customers](../api/bookingbusiness-update-customers.md)|[bookingCustomer](../resources/bookingcustomer.md)|Update the properties of a customers object.|
|[Get bookingCustomer](../api/bookingcustomer-get.md)|[bookingCustomer](../resources/bookingcustomer.md)|Read the properties and relationships of a [bookingCustomer](../resources/bookingcustomer.md) object.|
|[List services](../api/bookingbusiness-list-services.md)|[bookingService](../resources/bookingservice.md) collection|Get the bookingServices from the services navigation property.|
|[Create services](../api/bookingbusiness-post-services.md)|[bookingService](../resources/bookingservice.md)|Create a new services object.|
|[Delete services](../api/bookingbusiness-delete-services.md)|None|Delete a [bookingService](../resources/bookingservice.md) object.|
|[Update services](../api/bookingbusiness-update-services.md)|[bookingService](../resources/bookingservice.md)|Update the properties of a services object.|
|[Get bookingService](../api/bookingservice-get.md)|[bookingService](../resources/bookingservice.md)|Read the properties and relationships of a [bookingService](../resources/bookingservice.md) object.|
|[List staffMembers](../api/bookingbusiness-list-staffmembers.md)|[bookingStaffMember](../resources/bookingstaffmember.md) collection|Get the bookingStaffMembers from the staffMembers navigation property.|
|[Create staffMembers](../api/bookingbusiness-post-staffmembers.md)|[bookingStaffMember](../resources/bookingstaffmember.md)|Create a new staffMembers object.|
|[Delete staffMembers](../api/bookingbusiness-delete-staffmembers.md)|None|Delete a [bookingStaffMember](../resources/bookingstaffmember.md) object.|
|[Update staffMembers](../api/bookingbusiness-update-staffmembers.md)|[bookingStaffMember](../resources/bookingstaffmember.md)|Update the properties of a staffMembers object.|
|[Get bookingStaffMember](../api/bookingstaffmember-get.md)|[bookingStaffMember](../resources/bookingstaffmember.md)|Read the properties and relationships of a [bookingStaffMember](../resources/bookingstaffmember.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description**|
|businessHours|[bookingWorkHours](../resources/bookingworkhours.md) collection|**TODO: Add Description**|
|businessType|String|**TODO: Add Description**|
|defaultCurrencyIso|String|**TODO: Add Description**|
|displayName|String|Display name of this entity.
The display name is suitable for human-readable interfaces. Inherited from [bookingNamedEntity](../resources/bookingnamedentity.md)|
|email|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isPublished|Boolean|**TODO: Add Description**|
|phone|String|**TODO: Add Description**|
|publicUrl|String|**TODO: Add Description**|
|schedulingPolicy|[bookingSchedulingPolicy](../resources/bookingschedulingpolicy.md)|**TODO: Add Description**|
|webSiteUrl|String|The URL of the business web site.
Example: https://www.contoso.com|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appointments|[bookingAppointment](../resources/bookingappointment.md) collection|All appointments in this business.|
|calendarView|[bookingAppointment](../resources/bookingappointment.md) collection|A calendar view of appointments in this business.|
|customers|[bookingCustomer](../resources/bookingcustomer.md) collection|All customers of this business.|
|services|[bookingService](../resources/bookingservice.md) collection|All services offered by this business.|
|staffMembers|[bookingStaffMember](../resources/bookingstaffmember.md) collection|All staff members that provides services in this business.|

## JSON representation
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

