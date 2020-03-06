---
title: "calendarPermission resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# calendarPermission resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get calendarPermission](../api/calendarpermission-get.md)|[calendarPermission](../resources/calendarpermission.md)|Read properties and relationships of the [calendarPermission](../resources/calendarpermission.md) object.|
|[Update calendarPermission](../api/calendarpermission-update.md)|[calendarPermission](../resources/calendarpermission.md)|Update the properties of a [calendarPermission](../resources/calendarpermission.md) object.|
|[List calendarPermissions](../api/calendar-list-calendarpermissions.md)|[calendarPermission](../resources/calendarpermission.md) collection|Get the calendarPermissions from the calendarPermissions navigation property.|
|[Add calendarPermissions](../api/calendar-post-calendarpermissions.md)|[calendarPermission](../resources/calendarpermission.md)|Add calendarPermissions by posting to the calendarPermissions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedRoles|Enumeration collection||
|emailAddress|[emailAddress](../resources/emailaddress.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|isInsideOrganization|Boolean||
|isRemovable|Boolean||
|role|Enumeration|. Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.calendarPermission",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.calendarPermission",
  "id": "String (identifier)",
  "emailAddress": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "isRemovable": true,
  "isInsideOrganization": true,
  "role": "String",
  "allowedRoles": [
    "String"
  ]
}
```

