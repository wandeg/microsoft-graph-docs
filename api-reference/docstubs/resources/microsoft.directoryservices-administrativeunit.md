---
title: "administrativeUnit resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# administrativeUnit resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List administrativeUnits](../api/microsoft.directoryservices-administrativeunit-list.md)|[administrativeUnit](../resources/microsoft.directoryservices-administrativeunit.md) collection|Get a list of the [administrativeUnit](../resources/administrativeunit.md) objects and their properties.|
|[Get administrativeUnit](../api/microsoft.directoryservices-administrativeunit-get.md)|[administrativeUnit](../resources/microsoft.directoryservices-administrativeunit.md)|Read properties and relationships of an [administrativeUnit](../resources/microsoft.directoryservices-administrativeunit.md) object.|
|[Create administrativeUnit](../api/microsoft.directoryservices-administrativeunit-post-administrativeunits.md)|[administrativeUnit](../resources/microsoft.directoryservices-administrativeunit.md)|Create a new [administrativeUnit](../resources/microsoft.directoryservices-administrativeunit.md) object.|
|[Delete administrativeUnit](../api/microsoft.directoryservices-administrativeunit-delete.md)|None|Deletes an [administrativeUnit](../resources/microsoft.directoryservices-administrativeunit.md).|
|[Update administrativeUnit](../api/microsoft.directoryservices-administrativeunit-update.md)|[administrativeUnit](../resources/microsoft.directoryservices-administrativeunit.md)|Update the properties of a [administrativeUnit](../resources/microsoft.directoryservices-administrativeunit.md) object.|
|[delta](../api/microsoft.directoryservices-administrativeunit-delta.md)|[administrativeUnit](../resources/microsoft.directoryservices-administrativeunit.md) collection|**TODO: Add Description**|
|[checkMemberGroups](../api/microsoft.directoryservices-administrativeunit-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/microsoft.directoryservices-administrativeunit-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/microsoft.directoryservices-administrativeunit-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/microsoft.directoryservices-administrativeunit-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/microsoft.directoryservices-administrativeunit-restore.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|
|[List members](../api/microsoft.directoryservices-administrativeunit-list-members.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the members navigation property.|
|[Add members](../api/microsoft.directoryservices-administrativeunit-post-members.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add members by posting to the members collection.|
|[Remove members](../api/microsoft.directoryservices-administrativeunit-delete-members.md)|None|Remove a members object.|
|[List scopedRoleMembers](../api/microsoft.directoryservices-administrativeunit-list-scopedrolemembers.md)|[scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md) collection|Get the scopedRoleMemberships from the scopedRoleMembers navigation property.|
|[Create scopedRoleMembers](../api/microsoft.directoryservices-administrativeunit-post-scopedrolemembers.md)|[scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md)|Create a new scopedRoleMembers object.|
|[Delete scopedRoleMembers](../api/microsoft.directoryservices-administrativeunit-delete-scopedrolemembers.md)|None|Delete a scopedRoleMembers object.|
|[Update scopedRoleMembers](../api/microsoft.directoryservices-administrativeunit-update-scopedrolemembers.md)|[scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md)|Update the properties of a scopedRoleMembers object.|
|[Get scopedRoleMembership](../api/microsoft.directoryservices-scopedrolemembership-get.md)|[scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md)|Read properties and relationships of a [scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|visibility|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|members|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|
|scopedRoleMembers|[scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.administrativeUnit",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.administrativeUnit",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "visibility": "String"
}
```

