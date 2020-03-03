---
title: "onenote resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# onenote resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List onenotes](../api/onenote-list.md)|[onenote](../resources/onenote.md) collection|List properties and relationships of the [onenote](../resources/onenote.md) objects.|
|[Get onenote](../api/onenote-get.md)|[onenote](../resources/onenote.md)|Read properties and relationships of the [onenote](../resources/onenote.md) object.|
|[Create onenote](../api/onenote-create.md)|[onenote](../resources/onenote.md)|Create a new [onenote](../resources/onenote.md) object.|
|[Delete onenote](../api/onenote-delete.md)|None|Deletes a [onenote](../resources/onenote.md).|
|[Update onenote](../api/onenote-update.md)|[onenote](../resources/onenote.md)|Update the properties of a [onenote](../resources/onenote.md) object.|
|[List notebooks](../api/onenote-list-notebooks.md)|[notebook](../resources/notebook.md) collection|Get the notebooks from the notebooks navigation property.|
|[Add notebooks](../api/onenote-post-notebooks.md)|[notebook](../resources/notebook.md)|Add notebooks by posting to the notebooks collection.|
|[List sections](../api/onenote-list-sections.md)|[onenoteSection](../resources/onenoteSection.md) collection|Get the onenoteSections from the sections navigation property.|
|[Add sections](../api/onenote-post-sections.md)|[onenoteSection](../resources/onenoteSection.md)|Add sections by posting to the sections collection.|
|[List sectionGroups](../api/onenote-list-sectiongroups.md)|[sectionGroup](../resources/sectionGroup.md) collection|Get the sectionGroups from the sectionGroups navigation property.|
|[Add sectionGroups](../api/onenote-post-sectiongroups.md)|[sectionGroup](../resources/sectionGroup.md)|Add sectionGroups by posting to the sectionGroups collection.|
|[List pages](../api/onenote-list-pages.md)|[onenotePage](../resources/onenotePage.md) collection|Get the onenotePages from the pages navigation property.|
|[Add pages](../api/onenote-post-pages.md)|[onenotePage](../resources/onenotePage.md)|Add pages by posting to the pages collection.|
|[List resources](../api/onenote-list-resources.md)|[onenoteResource](../resources/onenoteResource.md) collection|Get the onenoteResources from the resources navigation property.|
|[Add resources](../api/onenote-post-resources.md)|[onenoteResource](../resources/onenoteResource.md)|Add resources by posting to the resources collection.|
|[List operations](../api/onenote-list-operations.md)|[onenoteOperation](../resources/onenoteOperation.md) collection|Get the onenoteOperations from the operations navigation property.|
|[Add operations](../api/onenote-post-operations.md)|[onenoteOperation](../resources/onenoteOperation.md)|Add operations by posting to the operations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|notebooks|[notebook](../resources/notebook.md) collection||
|operations|[onenoteOperation](../resources/onenoteOperation.md) collection||
|pages|[onenotePage](../resources/onenotePage.md) collection||
|resources|[onenoteResource](../resources/onenoteResource.md) collection||
|sectionGroups|[sectionGroup](../resources/sectionGroup.md) collection||
|sections|[onenoteSection](../resources/onenoteSection.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onenote",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenote",
  "id": "String (identifier)"
}
```

