---
title: "directoryRole resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# directoryRole resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List directoryRoles](../api/microsoft.directoryservices-directoryrole-list.md)|[directoryRole](../resources/microsoft.directoryservices-directoryrole.md) collection|Get a list of the [directoryRole](../resources/directoryrole.md) objects and their properties.|
|[Get directoryRole](../api/microsoft.directoryservices-directoryrole-get.md)|[directoryRole](../resources/microsoft.directoryservices-directoryrole.md)|Read properties and relationships of a [directoryRole](../resources/microsoft.directoryservices-directoryrole.md) object.|
|[Create directoryRole](../api/microsoft.directoryservices-directoryrole-post-directoryroles.md)|[directoryRole](../resources/microsoft.directoryservices-directoryrole.md)|Create a new [directoryRole](../resources/microsoft.directoryservices-directoryrole.md) object.|
|[Delete directoryRole](../api/microsoft.directoryservices-directoryrole-delete.md)|None|Deletes a [directoryRole](../resources/microsoft.directoryservices-directoryrole.md).|
|[Update directoryRole](../api/microsoft.directoryservices-directoryrole-update.md)|[directoryRole](../resources/microsoft.directoryservices-directoryrole.md)|Update the properties of a [directoryRole](../resources/microsoft.directoryservices-directoryrole.md) object.|
|[delta](../api/microsoft.directoryservices-directoryrole-delta.md)|[directoryRole](../resources/microsoft.directoryservices-directoryrole.md) collection|**TODO: Add Description**|
|[checkMemberGroups](../api/microsoft.directoryservices-directoryrole-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/microsoft.directoryservices-directoryrole-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/microsoft.directoryservices-directoryrole-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/microsoft.directoryservices-directoryrole-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/microsoft.directoryservices-directoryrole-restore.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|
|[List members](../api/microsoft.directoryservices-directoryrole-list-members.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the members navigation property.|
|[Add members](../api/microsoft.directoryservices-directoryrole-post-members.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Add members by posting to the members collection.|
|[Remove members](../api/microsoft.directoryservices-directoryrole-delete-members.md)|None|Remove a members object.|
|[List scopedMembers](../api/microsoft.directoryservices-directoryrole-list-scopedmembers.md)|[scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md) collection|Get the scopedRoleMemberships from the scopedMembers navigation property.|
|[Create scopedMembers](../api/microsoft.directoryservices-directoryrole-post-scopedmembers.md)|[scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md)|Create a new scopedMembers object.|
|[Delete scopedMembers](../api/microsoft.directoryservices-directoryrole-delete-scopedmembers.md)|None|Delete a scopedMembers object.|
|[Update scopedMembers](../api/microsoft.directoryservices-directoryrole-update-scopedmembers.md)|[scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md)|Update the properties of a scopedMembers object.|
|[Get scopedRoleMembership](../api/microsoft.directoryservices-scopedrolemembership-get.md)|[scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md)|Read properties and relationships of a [scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|roleTemplateId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|members|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|
|scopedMembers|[scopedRoleMembership](../resources/microsoft.directoryservices-scopedrolemembership.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.directoryRole",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.directoryRole",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "roleTemplateId": "String"
}
```

