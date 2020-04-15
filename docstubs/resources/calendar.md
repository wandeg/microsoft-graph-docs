---
title: "calendar resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# calendar resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get calendar](../api/calendar-get.md)|[calendar](../resources/calendar.md)|Read properties and relationships of a [calendar](../resources/calendar.md) object.|
|[Update calendar](../api/calendar-update.md)|[calendar](../resources/calendar.md)|Update the properties of a [calendar](../resources/calendar.md) object.|
|[getSchedule](../api/calendar-getschedule.md)|[scheduleInformation](../resources/scheduleinformation.md) collection|**TODO: Add Description**|
|[allowedCalendarSharingRoles](../api/calendar-allowedcalendarsharingroles.md)|calendarRoleType collection|**TODO: Add Description**|
|[List singleValueExtendedProperties](../api/calendar-list-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection|Get the singleValueLegacyExtendedProperties from the singleValueExtendedProperties navigation property.|
|[Add singleValueExtendedProperties](../api/calendar-post-singlevalueextendedproperties.md)|[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md)|Add singleValueExtendedProperties by posting to the singleValueExtendedProperties collection.|
|[List multiValueExtendedProperties](../api/calendar-list-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection|Get the multiValueLegacyExtendedProperties from the multiValueExtendedProperties navigation property.|
|[Add multiValueExtendedProperties](../api/calendar-post-multivalueextendedproperties.md)|[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)|Add multiValueExtendedProperties by posting to the multiValueExtendedProperties collection.|
|[List calendarPermissions](../api/calendar-list-calendarpermissions.md)|[calendarPermission](../resources/calendarpermission.md) collection|Get the calendarPermissions from the calendarPermissions navigation property.|
|[Add calendarPermissions](../api/calendar-post-calendarpermissions.md)|[calendarPermission](../resources/calendarpermission.md)|Add calendarPermissions by posting to the calendarPermissions collection.|
|[List events](../api/calendar-list-events.md)|[event](../resources/event.md) collection|Get the events from the events navigation property.|
|[Add events](../api/calendar-post-events.md)|[event](../resources/event.md)|Add events by posting to the events collection.|
|[List calendarView](../api/calendar-list-calendarview.md)|[event](../resources/event.md) collection|Get the events from the calendarView navigation property.|
|[Add calendarView](../api/calendar-post-calendarview.md)|[event](../resources/event.md)|Add calendarView by posting to the calendarView collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedOnlineMeetingProviders|onlineMeetingProviderType collection|**TODO: Add Description**|
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
  "isDefaultCalendar": true,
  "changeKey": "String",
  "canShare": true,
  "canViewPrivateItems": true,
  "isShared": true,
  "isSharedWithMe": true,
  "canEdit": true,
  "owner": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "allowedOnlineMeetingProviders": [
    "String"
  ],
  "defaultOnlineMeetingProvider": "String",
  "isTallyingResponses": true,
  "isRemovable": true
}
```

