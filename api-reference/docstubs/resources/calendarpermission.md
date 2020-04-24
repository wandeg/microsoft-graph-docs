---
title: "calendarPermission resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# calendarPermission resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get calendarPermission](../api/calendarpermission-get.md)|[calendarPermission](../resources/calendarpermission.md)|Read the properties and relationships of a [calendarPermission](../resources/calendarpermission.md) object.|
|[Update calendarPermission](../api/calendarpermission-update.md)|[calendarPermission](../resources/calendarpermission.md)|Update the properties of a [calendarPermission](../resources/calendarpermission.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedRoles|calendarRoleType collection|**TODO: Add Description**|
|emailAddress|[emailAddress](../resources/emailaddress.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isInsideOrganization|Boolean|**TODO: Add Description**|
|isRemovable|Boolean|**TODO: Add Description**|
|role|calendarRoleType|**TODO: Add Description**. Possible values are: `none`, `freeBusyRead`, `limitedRead`, `read`, `write`, `delegateWithoutPrivateEventAccess`, `delegateWithPrivateEventAccess`, `custom`.|

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

