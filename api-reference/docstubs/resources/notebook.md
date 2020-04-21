---
title: "notebook resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# notebook resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get notebook](../api/notebook-get.md)|[notebook](../resources/notebook.md)|Read properties and relationships of a [notebook](../resources/notebook.md) object.|
|[Update notebook](../api/notebook-update.md)|[notebook](../resources/notebook.md)|Update the properties of a [notebook](../resources/notebook.md) object.|
|[copyNotebook](../api/notebook-copynotebook.md)|[onenoteOperation](../resources/onenoteoperation.md)|**TODO: Add Description**|
|[getRecentNotebooks](../api/notebook-getrecentnotebooks.md)|[recentNotebook](../resources/recentnotebook.md) collection|**TODO: Add Description**|
|[getNotebookFromWebUrl](../api/notebook-getnotebookfromweburl.md)|[CopyNotebookModel](../resources/copynotebookmodel.md)|**TODO: Add Description**|
|[List sections](../api/notebook-list-sections.md)|[onenoteSection](../resources/onenotesection.md) collection|Get the onenoteSections from the sections navigation property.|
|[Create sections](../api/notebook-post-sections.md)|[onenoteSection](../resources/onenotesection.md)|Create a new sections object.|
|[Delete sections](../api/notebook-delete-sections.md)|None|Delete a sections object.|
|[Update sections](../api/notebook-update-sections.md)|[onenoteSection](../resources/onenotesection.md)|Update the properties of a sections object.|
|[Get onenoteSection](../api/onenotesection-get.md)|[onenoteSection](../resources/onenotesection.md)|Read properties and relationships of an [onenoteSection](../resources/onenotesection.md) object.|
|[List sectionGroups](../api/notebook-list-sectiongroups.md)|[sectionGroup](../resources/sectiongroup.md) collection|Get the sectionGroups from the sectionGroups navigation property.|
|[Create sectionGroups](../api/notebook-post-sectiongroups.md)|[sectionGroup](../resources/sectiongroup.md)|Create a new sectionGroups object.|
|[Delete sectionGroups](../api/notebook-delete-sectiongroups.md)|None|Delete a sectionGroups object.|
|[Update sectionGroups](../api/notebook-update-sectiongroups.md)|[sectionGroup](../resources/sectiongroup.md)|Update the properties of a sectionGroups object.|
|[Get sectionGroup](../api/sectiongroup-get.md)|[sectionGroup](../resources/sectiongroup.md)|Read properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.|
|[List notebooks](../api/onenote-list-notebooks.md)|[notebook](../resources/notebook.md) collection|Get the notebooks from the notebooks navigation property.|
|[Create notebooks](../api/onenote-post-notebooks.md)|[notebook](../resources/notebook.md)|Create a new notebooks object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)|
|displayName|String|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean|**TODO: Add Description**|
|isShared|Boolean|**TODO: Add Description**|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|links|[notebookLinks](../resources/notebooklinks.md)|**TODO: Add Description**|
|sectionGroupsUrl|String|**TODO: Add Description**|
|sectionsUrl|String|**TODO: Add Description**|
|self|String|**TODO: Add Description** Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|
|userRole|onenoteUserRole|**TODO: Add Description**. Possible values are: `Owner`, `Contributor`, `Reader`, `None`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|sectionGroups|[sectionGroup](../resources/sectiongroup.md) collection|**TODO: Add Description**|
|sections|[onenoteSection](../resources/onenotesection.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.notebook",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.notebook",
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
  "isDefault": true,
  "userRole": "String",
  "isShared": true,
  "sectionsUrl": "String",
  "sectionGroupsUrl": "String",
  "links": {
    "@odata.type": "microsoft.graph.notebookLinks"
  }
}
```

