---
title: "directoryObject resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# directoryObject resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List directoryObjects](../api/microsoft.directoryservices-directoryobject-list.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get a list of the [directoryObject](../resources/directoryobject.md) objects and their properties.|
|[Get directoryObject](../api/microsoft.directoryservices-directoryobject-get.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Read properties and relationships of a [directoryObject](../resources/microsoft.directoryservices-directoryobject.md) object.|
|[Create directoryObject](../api/microsoft.directoryservices-directoryobject-post-directoryobjects.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Create a new [directoryObject](../resources/microsoft.directoryservices-directoryobject.md) object.|
|[Delete directoryObject](../api/microsoft.directoryservices-directoryobject-delete.md)|None|Deletes a [directoryObject](../resources/microsoft.directoryservices-directoryobject.md).|
|[Update directoryObject](../api/microsoft.directoryservices-directoryobject-update.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Update the properties of a [directoryObject](../resources/microsoft.directoryservices-directoryobject.md) object.|
|[getByIds](../api/microsoft.directoryservices-directoryobject-getbyids.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|
|[checkMemberGroups](../api/microsoft.directoryservices-directoryobject-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/microsoft.directoryservices-directoryobject-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/microsoft.directoryservices-directoryobject-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/microsoft.directoryservices-directoryobject-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[validateProperties](../api/microsoft.directoryservices-directoryobject-validateproperties.md)|None|**TODO: Add Description**|
|[restore](../api/microsoft.directoryservices-directoryobject-restore.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|
|[getUserOwnedObjects](../api/microsoft.directoryservices-directoryobject-getuserownedobjects.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.directoryObject",
  "baseType": "",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.directoryObject",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)"
}
```

