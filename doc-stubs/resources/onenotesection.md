---
title: "onenoteSection resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# onenoteSection resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List sections](../api/onenote-list-sections.md)|[onenoteSection](../resources/onenotesection.md) collection|Get the onenoteSections from the sections navigation property.|
|[Create sections](../api/onenote-post-sections.md)|[onenoteSection](../resources/onenotesection.md)|Create a new sections object.|
|[Delete sections](../api/onenote-delete-sections.md)|None|Delete an [onenoteSection](../resources/onenotesection.md) object.|
|[Update sections](../api/onenote-update-sections.md)|[onenoteSection](../resources/onenotesection.md)|Update the properties of a sections object.|
|[Get sections](../api/onenote-get-onenotesection.md)|[onenoteSection](../resources/onenotesection.md)|Read the properties and relationships of an [onenoteSection](../resources/onenotesection.md) object.|
|[copyToNotebook](../api/onenotesection-copytonotebook.md)|[onenoteOperation](../resources/onenoteoperation.md)|**TODO: Add Description**|
|[copyToSectionGroup](../api/onenotesection-copytosectiongroup.md)|[onenoteOperation](../resources/onenoteoperation.md)|**TODO: Add Description**|
|[List parentNotebook](../api/onenotesection-list-parentnotebook.md)|[notebook](../resources/notebook.md) collection|Get the notebooks from the parentNotebook navigation property.|
|[Create parentNotebook](../api/onenotesection-post-parentnotebook.md)|[notebook](../resources/notebook.md)|Create a new parentNotebook object.|
|[Delete parentNotebook](../api/onenotesection-delete-parentnotebook.md)|None|Delete a [notebook](../resources/notebook.md) object.|
|[Update parentNotebook](../api/onenotesection-update-parentnotebook.md)|[notebook](../resources/notebook.md)|Update the properties of a parentNotebook object.|
|[Get parentNotebook](../api/onenotesection-get-notebook.md)|[notebook](../resources/notebook.md)|Read the properties and relationships of a [notebook](../resources/notebook.md) object.|
|[List parentSectionGroup](../api/onenotesection-list-parentsectiongroup.md)|[sectionGroup](../resources/sectiongroup.md) collection|Get the sectionGroups from the parentSectionGroup navigation property.|
|[Create parentSectionGroup](../api/onenotesection-post-parentsectiongroup.md)|[sectionGroup](../resources/sectiongroup.md)|Create a new parentSectionGroup object.|
|[Delete parentSectionGroup](../api/onenotesection-delete-parentsectiongroup.md)|None|Delete a [sectionGroup](../resources/sectiongroup.md) object.|
|[Update parentSectionGroup](../api/onenotesection-update-parentsectiongroup.md)|[sectionGroup](../resources/sectiongroup.md)|Update the properties of a parentSectionGroup object.|
|[Get parentSectionGroup](../api/onenotesection-get-sectiongroup.md)|[sectionGroup](../resources/sectiongroup.md)|Read the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.|
|[List pages](../api/onenotesection-list-pages.md)|[onenotePage](../resources/onenotepage.md) collection|Get the onenotePages from the pages navigation property.|
|[Create pages](../api/onenotesection-post-pages.md)|[onenotePage](../resources/onenotepage.md)|Create a new pages object.|
|[Delete pages](../api/onenotesection-delete-pages.md)|None|Delete an [onenotePage](../resources/onenotepage.md) object.|
|[Update pages](../api/onenotesection-update-pages.md)|[onenotePage](../resources/onenotepage.md)|Update the properties of a pages object.|
|[Get pages](../api/onenotesection-get-onenotepage.md)|[onenotePage](../resources/onenotepage.md)|Read the properties and relationships of an [onenotePage](../resources/onenotepage.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)|
|displayName|String|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean|**TODO: Add Description**|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|links|[sectionLinks](../resources/sectionlinks.md)|**TODO: Add Description**|
|pagesUrl|String|**TODO: Add Description**|
|self|String|**TODO: Add Description** Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|pages|[onenotePage](../resources/onenotepage.md) collection|**TODO: Add Description**|
|parentNotebook|[notebook](../resources/notebook.md)|**TODO: Add Description**|
|parentSectionGroup|[sectionGroup](../resources/sectiongroup.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onenoteSection",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenoteSection",
  "id": "String (identifier)",
  "self": "String",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "isDefault": "Boolean",
  "links": {
    "@odata.type": "microsoft.graph.sectionLinks"
  },
  "pagesUrl": "String"
}
```

