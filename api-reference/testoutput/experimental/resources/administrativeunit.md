---
title: "administrativeUnit resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# administrativeUnit resource type


Namespace: microsoft.graph

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List administrativeUnits](../api/administrativeunit-list.md)|[administrativeUnit](../resources/administrativeunit.md) collection|List properties and relationships of the [administrativeUnit](../resources/administrativeunit.md) objects.|
|[Get administrativeUnit](../api/administrativeunit-get.md)|[administrativeUnit](../resources/administrativeunit.md)|Read properties and relationships of the [administrativeUnit](../resources/administrativeunit.md) object.|
|[Create administrativeUnit](../api/administrativeunit-post-administrativeunits.md)|[administrativeUnit](../resources/administrativeunit.md)|Create a new [administrativeUnit](../resources/administrativeunit.md) object.|
|[Delete administrativeUnit](../api/administrativeunit-delete.md)|None|Deletes a [administrativeUnit](../resources/administrativeunit.md).|
|[Update administrativeUnit](../api/administrativeunit-update.md)|[administrativeUnit](../resources/administrativeunit.md)|Update the properties of a [administrativeUnit](../resources/administrativeunit.md) object.|
|[delta](../api/administrativeunit-delta.md)|[administrativeUnit](../resources/administrativeunit.md) collection||
|[checkMemberGroups](../api/administrativeunit-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/administrativeunit-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/administrativeunit-getmembergroups.md)|String collection||
|[getMemberObjects](../api/administrativeunit-getmemberobjects.md)|String collection||
|[restore](../api/administrativeunit-restore.md)|[directoryObject](../resources/directoryobject.md)||
|[List members](../api/administrativeunit-list-members.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the members navigation property.|
|[Create members](../api/administrativeunit-post-members.md)|[directoryObject](../resources/directoryobject.md)|Create members by posting to the members collection.|
|[List scopedRoleMembers](../api/administrativeunit-list-scopedrolemembers.md)|[scopedRoleMembership](../resources/scopedrolemembership.md) collection|Get the scopedRoleMemberships from the scopedRoleMembers navigation property.|
|[Add scopedRoleMembers](../api/administrativeunit-post-scopedrolemembers.md)|[scopedRoleMembership](../resources/scopedrolemembership.md)|Add scopedRoleMembers by posting to the scopedRoleMembers collection.|
|[List extensions](../api/administrativeunit-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extensions from the extensions navigation property.|
|[Add extensions](../api/administrativeunit-post-extensions.md)|[extension](../resources/extension.md)|Add extensions by posting to the extensions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|visibility|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|extensions|[extension](../resources/extension.md) collection||
|members|[directoryObject](../resources/directoryobject.md) collection||
|scopedRoleMembers|[scopedRoleMembership](../resources/scopedrolemembership.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.administrativeUnit",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.administrativeUnit",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "visibility": "String"
}
```

