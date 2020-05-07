---
title: "sectionGroup resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# sectionGroup resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List parentNotebook](../api/sectiongroup-list-parentnotebook.md)|[notebook](../resources/notebook.md) collection|Get the notebooks from the parentNotebook navigation property.|
|[Create parentNotebook](../api/sectiongroup-post-parentnotebook.md)|[notebook](../resources/notebook.md)|Create a new parentNotebook object.|
|[Delete parentNotebook](../api/sectiongroup-delete-parentnotebook.md)|None|Delete a [notebook](../resources/notebook.md) object.|
|[Update parentNotebook](../api/sectiongroup-update-parentnotebook.md)|[notebook](../resources/notebook.md)|Update the properties of a parentNotebook object.|
|[Get notebook](../api/notebook-get.md)|[notebook](../resources/notebook.md)|Read the properties and relationships of a [notebook](../resources/notebook.md) object.|
|[List parentSectionGroup](../api/sectiongroup-list-parentsectiongroup.md)|[sectionGroup](../resources/sectiongroup.md) collection|Get the sectionGroups from the parentSectionGroup navigation property.|
|[Create parentSectionGroup](../api/sectiongroup-post-parentsectiongroup.md)|[sectionGroup](../resources/sectiongroup.md)|Create a new parentSectionGroup object.|
|[Delete parentSectionGroup](../api/sectiongroup-delete-parentsectiongroup.md)|None|Delete a [sectionGroup](../resources/sectiongroup.md) object.|
|[Update parentSectionGroup](../api/sectiongroup-update-parentsectiongroup.md)|[sectionGroup](../resources/sectiongroup.md)|Update the properties of a parentSectionGroup object.|
|[Get sectionGroup](../api/sectiongroup-get.md)|[sectionGroup](../resources/sectiongroup.md)|Read the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.|
|[List sections](../api/sectiongroup-list-sections.md)|[onenoteSection](../resources/onenotesection.md) collection|Get the onenoteSections from the sections navigation property.|
|[Create sections](../api/sectiongroup-post-sections.md)|[onenoteSection](../resources/onenotesection.md)|Create a new sections object.|
|[Delete sections](../api/sectiongroup-delete-sections.md)|None|Delete a [onenoteSection](../resources/onenotesection.md) object.|
|[Update sections](../api/sectiongroup-update-sections.md)|[onenoteSection](../resources/onenotesection.md)|Update the properties of a sections object.|
|[Get onenoteSection](../api/onenotesection-get.md)|[onenoteSection](../resources/onenotesection.md)|Read the properties and relationships of an [onenoteSection](../resources/onenotesection.md) object.|
|[List sectionGroups](../api/sectiongroup-list-sectiongroups.md)|[sectionGroup](../resources/sectiongroup.md) collection|Get the sectionGroups from the sectionGroups navigation property.|
|[Create sectionGroups](../api/sectiongroup-post-sectiongroups.md)|[sectionGroup](../resources/sectiongroup.md)|Create a new sectionGroups object.|
|[Delete sectionGroups](../api/sectiongroup-delete-sectiongroups.md)|None|Delete a [sectionGroup](../resources/sectiongroup.md) object.|
|[Update sectionGroups](../api/sectiongroup-update-sectiongroups.md)|[sectionGroup](../resources/sectiongroup.md)|Update the properties of a sectionGroups object.|
|[Get sectionGroup](../api/sectiongroup-get.md)|[sectionGroup](../resources/sectiongroup.md)|Read the properties and relationships of a [sectionGroup](../resources/sectiongroup.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)|
|displayName|String|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [onenoteEntityHierarchyModel](../resources/onenoteentityhierarchymodel.md)|
|sectionGroupsUrl|String|**TODO: Add Description**|
|sectionsUrl|String|**TODO: Add Description**|
|self|String|**TODO: Add Description** Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|parentNotebook|[notebook](../resources/notebook.md)|**TODO: Add Description**|
|parentSectionGroup|[sectionGroup](../resources/sectiongroup.md)|**TODO: Add Description**|
|sectionGroups|[sectionGroup](../resources/sectiongroup.md) collection|**TODO: Add Description**|
|sections|[onenoteSection](../resources/onenotesection.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sectionGroup",
  "baseType": "microsoft.graph.onenoteEntityHierarchyModel",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sectionGroup",
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
  "sectionsUrl": "String",
  "sectionGroupsUrl": "String"
}
```

