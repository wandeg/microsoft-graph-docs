---
title: "directoryRoleTemplate resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# directoryRoleTemplate resource type


Namespace: microsoft.graph

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List directoryRoleTemplates](../api/directoryroletemplate-list.md)|[directoryRoleTemplate](../resources/directoryroletemplate.md) collection|Get a list of the [directoryRoleTemplate](../resources/directoryroletemplate.md) objects and their properties.|
|[Get directoryRoleTemplate](../api/directoryroletemplate-get.md)|[directoryRoleTemplate](../resources/directoryroletemplate.md)|Read properties and relationships of a [directoryRoleTemplate](../resources/directoryroletemplate.md) object.|
|[Create directoryRoleTemplate](../api/directoryroletemplate-post-directoryroletemplates.md)|[directoryRoleTemplate](../resources/directoryroletemplate.md)|Create a new [directoryRoleTemplate](../resources/directoryroletemplate.md) object.|
|[Delete directoryRoleTemplate](../api/directoryroletemplate-delete.md)|None|Deletes a [directoryRoleTemplate](../resources/directoryroletemplate.md).|
|[Update directoryRoleTemplate](../api/directoryroletemplate-update.md)|[directoryRoleTemplate](../resources/directoryroletemplate.md)|Update the properties of a [directoryRoleTemplate](../resources/directoryroletemplate.md) object.|
|[checkMemberGroups](../api/directoryroletemplate-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/directoryroletemplate-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/directoryroletemplate-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/directoryroletemplate-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/directoryroletemplate-restore.md)|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.directoryRoleTemplate",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String"
}
```

