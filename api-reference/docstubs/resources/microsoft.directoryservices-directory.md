---
title: "directory resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# directory resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get directory](../api/microsoft.directoryservices-directory-get.md)|[directory](../resources/microsoft.directoryservices-directory.md)|Read properties and relationships of a [directory](../resources/microsoft.directoryservices-directory.md) object.|
|[Update directory](../api/microsoft.directoryservices-directory-update.md)|[directory](../resources/microsoft.directoryservices-directory.md)|Update the properties of a [directory](../resources/microsoft.directoryservices-directory.md) object.|
|[List deletedItems](../api/microsoft.directoryservices-directory-list-deleteditems.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|Get the directoryObjects from the deletedItems navigation property.|
|[Create deletedItems](../api/microsoft.directoryservices-directory-post-deleteditems.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Create a new deletedItems object.|
|[Delete deletedItems](../api/microsoft.directoryservices-directory-delete-deleteditems.md)|None|Delete a deletedItems object.|
|[Update deletedItems](../api/microsoft.directoryservices-directory-update-deleteditems.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Update the properties of a deletedItems object.|
|[Get directoryObject](../api/microsoft.directoryservices-directoryobject-get.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|Read properties and relationships of a [directoryObject](../resources/microsoft.directoryservices-directoryobject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deletedItems|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.directory",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.directory"
}
```

