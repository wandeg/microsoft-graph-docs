---
title: "directoryRole resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# directoryRole resource type


Namespace: microsoft.graph

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List directoryRoles](../api/directoryrole-list.md)|[directoryRole](../resources/directoryrole.md) collection|Get a list of the [directoryRole](../resources/directoryrole.md) objects and their properties.|
|[Get directoryRole](../api/directoryrole-get.md)|[directoryRole](../resources/directoryrole.md)|Read properties and relationships of a [directoryRole](../resources/directoryrole.md) object.|
|[Create directoryRole](../api/directoryrole-post-directoryroles.md)|[directoryRole](../resources/directoryrole.md)|Create a new [directoryRole](../resources/directoryrole.md) object.|
|[Delete directoryRole](../api/directoryrole-delete.md)|None|Deletes a [directoryRole](../resources/directoryrole.md).|
|[Update directoryRole](../api/directoryrole-update.md)|[directoryRole](../resources/directoryrole.md)|Update the properties of a [directoryRole](../resources/directoryrole.md) object.|
|[delta](../api/directoryrole-delta.md)|[directoryRole](../resources/directoryrole.md) collection|**TODO: Add Description**|
|[checkMemberGroups](../api/directoryrole-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/directoryrole-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/directoryrole-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/directoryrole-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/directoryrole-restore.md)|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|[List members](../api/directoryrole-list-members.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the members navigation property.|
|[Add members](../api/directoryrole-post-members.md)|[directoryObject](../resources/directoryobject.md)|Add members by posting to the members collection.|
|[Remove members](../api/directoryrole-delete-members.md)|None|Remove a members object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|roleTemplateId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|members|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRole",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.directoryRole",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "roleTemplateId": "String"
}
```

