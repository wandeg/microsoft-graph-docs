---
title: "onenote resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# onenote resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List notebooks](../api/onenote-list-notebooks.md)|[notebook](../resources/notebook.md) collection|Get the notebooks from the notebooks navigation property.|
|[Create notebooks](../api/onenote-post-notebooks.md)|[notebook](../resources/notebook.md)|Create a new notebooks object.|
|[Delete notebooks](../api/onenote-delete-notebooks.md)|None|Delete a [notebook](../resources/notebook.md) object.|
|[Update notebooks](../api/onenote-update-notebooks.md)|[notebook](../resources/notebook.md)|Update the properties of a notebooks object.|
|[Get notebook](../api/notebook-get.md)|[notebook](../resources/notebook.md)|Read the properties and relationships of a [notebook](../resources/notebook.md) object.|
|[List sections](../api/onenote-list-sections.md)|[onenoteSection](../resources/onenotesection.md) collection|Get the onenoteSections from the sections navigation property.|
|[Create sections](../api/onenote-post-sections.md)|[onenoteSection](../resources/onenotesection.md)|Create a new sections object.|
|[Delete sections](../api/onenote-delete-sections.md)|None|Delete a [onenoteSection](../resources/onenotesection.md) object.|
|[Update sections](../api/onenote-update-sections.md)|[onenoteSection](../resources/onenotesection.md)|Update the properties of a sections object.|
|[Get onenoteSection](../api/onenotesection-get.md)|[onenoteSection](../resources/onenotesection.md)|Read the properties and relationships of an [onenoteSection](../resources/onenotesection.md) object.|
|[List sectionGroups](../api/onenote-list-sectiongroups.md)|[sectionGroup](../resources/sectiongroup.md) collection|Get the sectionGroups from the sectionGroups navigation property.|
|[Create sectionGroups](../api/onenote-post-sectiongroups.md)|[sectionGroup](../resources/sectiongroup.md)|Create a new sectionGroups object.|
|[Delete sectionGroups](../api/onenote-delete-sectiongroups.md)|None|Delete a [sectionGroup](../resources/sectiongroup.md) object.|
|[Update sectionGroups](../api/onenote-update-sectiongroups.md)|[sectionGroup](../resources/sectiongroup.md)|Update the properties of a sectionGroups object.|
|[Get sectionGroup](../api/sectiongroup-get.md)|[sectionGroup](../resources/sectiongroup.md)|Read the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.|
|[List pages](../api/onenote-list-pages.md)|[onenotePage](../resources/onenotepage.md) collection|Get the onenotePages from the pages navigation property.|
|[Create pages](../api/onenote-post-pages.md)|[onenotePage](../resources/onenotepage.md)|Create a new pages object.|
|[Delete pages](../api/onenote-delete-pages.md)|None|Delete a [onenotePage](../resources/onenotepage.md) object.|
|[Update pages](../api/onenote-update-pages.md)|[onenotePage](../resources/onenotepage.md)|Update the properties of a pages object.|
|[Get onenotePage](../api/onenotepage-get.md)|[onenotePage](../resources/onenotepage.md)|Read the properties and relationships of an [onenotePage](../resources/onenotepage.md) object.|
|[List resources](../api/onenote-list-resources.md)|[onenoteResource](../resources/onenoteresource.md) collection|Get the onenoteResources from the resources navigation property.|
|[Create resources](../api/onenote-post-resources.md)|[onenoteResource](../resources/onenoteresource.md)|Create a new resources object.|
|[Delete resources](../api/onenote-delete-resources.md)|None|Delete a [onenoteResource](../resources/onenoteresource.md) object.|
|[Update resources](../api/onenote-update-resources.md)|[onenoteResource](../resources/onenoteresource.md)|Update the properties of a resources object.|
|[Get onenoteResource](../api/onenoteresource-get.md)|[onenoteResource](../resources/onenoteresource.md)|Read the properties and relationships of an [onenoteResource](../resources/onenoteresource.md) object.|
|[List operations](../api/onenote-list-operations.md)|[onenoteOperation](../resources/onenoteoperation.md) collection|Get the onenoteOperations from the operations navigation property.|
|[Create operations](../api/onenote-post-operations.md)|[onenoteOperation](../resources/onenoteoperation.md)|Create a new operations object.|
|[Delete operations](../api/onenote-delete-operations.md)|None|Delete an [onenoteOperation](../resources/onenoteoperation.md) object.|
|[Update operations](../api/onenote-update-operations.md)|[onenoteOperation](../resources/onenoteoperation.md)|Update the properties of an operations object.|
|[Get onenoteOperation](../api/onenoteoperation-get.md)|[onenoteOperation](../resources/onenoteoperation.md)|Read the properties and relationships of an [onenoteOperation](../resources/onenoteoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|notebooks|[notebook](../resources/notebook.md) collection|**TODO: Add Description**|
|operations|[onenoteOperation](../resources/onenoteoperation.md) collection|**TODO: Add Description**|
|pages|[onenotePage](../resources/onenotepage.md) collection|**TODO: Add Description**|
|resources|[onenoteResource](../resources/onenoteresource.md) collection|**TODO: Add Description**|
|sectionGroups|[sectionGroup](../resources/sectiongroup.md) collection|**TODO: Add Description**|
|sections|[onenoteSection](../resources/onenotesection.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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

