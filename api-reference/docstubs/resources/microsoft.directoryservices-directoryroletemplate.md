---
title: "directoryRoleTemplate resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# directoryRoleTemplate resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List directoryRoleTemplates](../api/microsoft.directoryservices-directoryroletemplate-list.md)|[directoryRoleTemplate](../resources/microsoft.directoryservices-directoryroletemplate.md) collection|Get a list of the [directoryRoleTemplate](../resources/directoryroletemplate.md) objects and their properties.|
|[Get directoryRoleTemplate](../api/microsoft.directoryservices-directoryroletemplate-get.md)|[directoryRoleTemplate](../resources/microsoft.directoryservices-directoryroletemplate.md)|Read properties and relationships of a [directoryRoleTemplate](../resources/microsoft.directoryservices-directoryroletemplate.md) object.|
|[Create directoryRoleTemplate](../api/microsoft.directoryservices-directoryroletemplate-post-directoryroletemplates.md)|[directoryRoleTemplate](../resources/microsoft.directoryservices-directoryroletemplate.md)|Create a new [directoryRoleTemplate](../resources/microsoft.directoryservices-directoryroletemplate.md) object.|
|[Delete directoryRoleTemplate](../api/microsoft.directoryservices-directoryroletemplate-delete.md)|None|Deletes a [directoryRoleTemplate](../resources/microsoft.directoryservices-directoryroletemplate.md).|
|[Update directoryRoleTemplate](../api/microsoft.directoryservices-directoryroletemplate-update.md)|[directoryRoleTemplate](../resources/microsoft.directoryservices-directoryroletemplate.md)|Update the properties of a [directoryRoleTemplate](../resources/microsoft.directoryservices-directoryroletemplate.md) object.|
|[checkMemberGroups](../api/microsoft.directoryservices-directoryroletemplate-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/microsoft.directoryservices-directoryroletemplate-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/microsoft.directoryservices-directoryroletemplate-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/microsoft.directoryservices-directoryroletemplate-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/microsoft.directoryservices-directoryroletemplate-restore.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.directoryRoleTemplate",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.directoryRoleTemplate",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String"
}
```

