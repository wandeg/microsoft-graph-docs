---
title: "directory resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# directory resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List directories](../api/directory-list.md)|[directory](../resources/directory.md) collection|Get a list of the [directory](../resources/directory.md) objects and their properties.|
|[Create directory](../api/directory-create.md)|[directory](../resources/directory.md)|Create a new [directory](../resources/directory.md) object.|
|[Get directory](../api/directory-get.md)|[directory](../resources/directory.md)|Read the properties and relationships of a [directory](../resources/directory.md) object.|
|[Update directory](../api/directory-update.md)|[directory](../resources/directory.md)|Update the properties of a [directory](../resources/directory.md) object.|
|[Delete directory](../api/directory-delete.md)|None|Deletes a [directory](../resources/directory.md) object.|
|[List deletedItems](../api/directory-list-deleteditems.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObjects from the deletedItems navigation property.|
|[Create deletedItems](../api/directory-post-deleteditems.md)|[directoryObject](../resources/directoryobject.md)|Create a new deletedItems object.|
|[Get deletedItems](../api/directory-get-directoryobject.md)|[directoryObject](../resources/directoryobject.md)|Read the properties and relationships of a [directoryObject](../resources/directoryobject.md) object.|
|[Update deletedItems](../api/directory-update-deleteditems.md)|[directoryObject](../resources/directoryobject.md)|Update the properties of a deletedItems object.|
|[Delete deletedItems](../api/directory-delete-deleteditems.md)|None|Delete a [directoryObject](../resources/directoryobject.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deletedItems|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.directory",
  "id": "String (identifier)"
}
```

