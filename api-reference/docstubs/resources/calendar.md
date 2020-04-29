---
title: "calendar resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# calendar resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[getSchedule](../api/calendar-getschedule.md)|[scheduleInformation](../resources/scheduleinformation.md) collection|**TODO: Add Description**|
|[allowedCalendarSharingRoles](../api/calendar-allowedcalendarsharingroles.md)|calendarRoleType collection|**TODO: Add Description**|
|[List singleValueExtendedProperties](../api/calendar-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Create singleValueExtendedProperties](../api/calendar-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Create a new singleValueExtendedProperties object.|
|[Delete singleValueExtendedProperties](../api/calendar-delete-singlevalueextendedproperties.md)|None|Delete a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.|
|[Update singleValueExtendedProperties](../api/calendar-update-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Update the properties of a singleValueExtendedProperties object.|
|[Get singleValueLegacyExtendedProperty](../api/singlevaluelegacyextendedproperty-get.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Read the properties and relationships of a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.|
|[List multiValueExtendedProperties](../api/calendar-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Create multiValueExtendedProperties](../api/calendar-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Create a new multiValueExtendedProperties object.|
|[Delete multiValueExtendedProperties](../api/calendar-delete-multivalueextendedproperties.md)|None|Delete a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.|
|[Update multiValueExtendedProperties](../api/calendar-update-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Update the properties of a multiValueExtendedProperties object.|
|[Get multiValueLegacyExtendedProperty](../api/multivaluelegacyextendedproperty-get.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Read the properties and relationships of a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.|
|[List calendarPermissions](../api/calendar-list-calendarpermissions.md)|[calendarPermission](../resources/calendarpermission.md) collection|Get the calendarPermissions from the calendarPermissions navigation property.|
|[Create calendarPermissions](../api/calendar-post-calendarpermissions.md)|[calendarPermission](../resources/calendarpermission.md)|Create a new calendarPermissions object.|
|[Delete calendarPermissions](../api/calendar-delete-calendarpermissions.md)|None|Delete a [calendarPermission](../resources/calendarpermission.md) object.|
|[Update calendarPermissions](../api/calendar-update-calendarpermissions.md)|[calendarPermission](../resources/calendarpermission.md)|Update the properties of a calendarPermissions object.|
|[Get calendarPermission](../api/calendarpermission-get.md)|[calendarPermission](../resources/calendarpermission.md)|Read the properties and relationships of a [calendarPermission](../resources/calendarpermission.md) object.|
|[List events](../api/calendar-list-events.md)|[event](../resources/event.md) collection|Get the events from the events navigation property.|
|[Create events](../api/calendar-post-events.md)|[event](../resources/event.md)|Create a new events object.|
|[Delete events](../api/calendar-delete-events.md)|None|Delete an [event](../resources/event.md) object.|
|[Update events](../api/calendar-update-events.md)|[event](../resources/event.md)|Update the properties of an events object.|
|[Get event](../api/event-get.md)|[event](../resources/event.md)|Read the properties and relationships of an [event](../resources/event.md) object.|
|[List calendarView](../api/calendar-list-calendarview.md)|[event](../resources/event.md) collection|Get the events from the calendarView navigation property.|
|[Create calendarView](../api/calendar-post-calendarview.md)|[event](../resources/event.md)|Create a new calendarView object.|
|[Delete calendarView](../api/calendar-delete-calendarview.md)|None|Delete a [event](../resources/event.md) object.|
|[Update calendarView](../api/calendar-update-calendarview.md)|[event](../resources/event.md)|Update the properties of a calendarView object.|
|[Get event](../api/event-get.md)|[event](../resources/event.md)|Read the properties and relationships of an [event](../resources/event.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedOnlineMeetingProviders|onlineMeetingProviderType collection|**TODO: Add Description**|
|calendarGroupId|String|**TODO: Add Description**|
|canEdit|Boolean|**TODO: Add Description**|
|canShare|Boolean|**TODO: Add Description**|
|canViewPrivateItems|Boolean|**TODO: Add Description**|
|changeKey|String|**TODO: Add Description**|
|color|calendarColor|**TODO: Add Description**. Possible values are: `lightBlue`, `lightGreen`, `lightOrange`, `lightGray`, `lightYellow`, `lightTeal`, `lightPink`, `lightBrown`, `lightRed`, `maxColor`, `auto`.|
|defaultOnlineMeetingProvider|onlineMeetingProviderType|**TODO: Add Description**. Possible values are: `unknown`, `skypeForBusiness`, `skypeForConsumer`, `teamsForBusiness`.|
|hexColor|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isDefaultCalendar|Boolean|**TODO: Add Description**|
|isRemovable|Boolean|**TODO: Add Description**|
|isShared|Boolean|**TODO: Add Description**|
|isSharedWithMe|Boolean|**TODO: Add Description**|
|isTallyingResponses|Boolean|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|owner|[emailAddress](../resources/emailaddress.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|calendarPermissions|[calendarPermission](../resources/calendarpermission.md) collection|**TODO: Add Description**|
|calendarView|[event](../resources/event.md) collection|**TODO: Add Description**|
|events|[event](../resources/event.md) collection|**TODO: Add Description**|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|**TODO: Add Description**|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendar",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.calendar",
  "id": "String (identifier)",
  "name": "String",
  "color": "String",
  "hexColor": "String",
  "isDefaultCalendar": "Boolean",
  "changeKey": "String",
  "canShare": "Boolean",
  "canViewPrivateItems": "Boolean",
  "isShared": "Boolean",
  "isSharedWithMe": "Boolean",
  "canEdit": "Boolean",
  "owner": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "calendarGroupId": "String",
  "allowedOnlineMeetingProviders": [
    "String"
  ],
  "defaultOnlineMeetingProvider": "String",
  "isTallyingResponses": "Boolean",
  "isRemovable": "Boolean"
}
```

