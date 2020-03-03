---
title: "calendarPermission resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# calendarPermission resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get calendarPermission](../api/calendarpermission-get.md)|[calendarPermission](../resources/calendarPermission.md)|Read properties and relationships of the [calendarPermission](../resources/calendarpermission.md) object.|
|[Delete calendarPermission](../api/calendarpermission-delete.md)|None|Deletes a [calendarPermission](../resources/calendarpermission.md).|
|[Update calendarPermission](../api/calendarpermission-update.md)|[calendarPermission](../resources/calendarPermission.md)|Update the properties of a [calendarPermission](../resources/calendarpermission.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedRoles|Enumeration collection||
|emailAddress|[emailAddress](../resources/emailAddress.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|isInsideOrganization|Boolean||
|isRemovable|Boolean||
|role|Enumeration|. Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|

## Relationships
None

## JSON Representation
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

