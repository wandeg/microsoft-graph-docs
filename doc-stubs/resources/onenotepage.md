---
title: "onenotePage resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# onenotePage resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[onenotePatchContent](../api/onenotepage-onenotepatchcontent.md)|None|**TODO: Add Description**|
|[preview](../api/onenotepage-preview.md)|[onenotePagePreview](../resources/onenotepagepreview.md)|**TODO: Add Description**|
|[copyToSection](../api/onenotepage-copytosection.md)|[onenoteOperation](../resources/onenoteoperation.md)|**TODO: Add Description**|
|[List parentSection](../api/onenotepage-list-parentsection.md)|[onenoteSection](../resources/onenotesection.md) collection|Get the onenoteSections from the parentSection navigation property.|
|[Create parentSection](../api/onenotepage-post-parentsection.md)|[onenoteSection](../resources/onenotesection.md)|Create a new parentSection object.|
|[Delete parentSection](../api/onenotepage-delete-parentsection.md)|None|Delete a [onenoteSection](../resources/onenotesection.md) object.|
|[Update parentSection](../api/onenotepage-update-parentsection.md)|[onenoteSection](../resources/onenotesection.md)|Update the properties of a parentSection object.|
|[Get onenoteSection](../api/onenotesection-get.md)|[onenoteSection](../resources/onenotesection.md)|Read the properties and relationships of an [onenoteSection](../resources/onenotesection.md) object.|
|[List parentNotebook](../api/onenotepage-list-parentnotebook.md)|[notebook](../resources/notebook.md) collection|Get the notebooks from the parentNotebook navigation property.|
|[Create parentNotebook](../api/onenotepage-post-parentnotebook.md)|[notebook](../resources/notebook.md)|Create a new parentNotebook object.|
|[Delete parentNotebook](../api/onenotepage-delete-parentnotebook.md)|None|Delete a [notebook](../resources/notebook.md) object.|
|[Update parentNotebook](../api/onenotepage-update-parentnotebook.md)|[notebook](../resources/notebook.md)|Update the properties of a parentNotebook object.|
|[Get notebook](../api/notebook-get.md)|[notebook](../resources/notebook.md)|Read the properties and relationships of a [notebook](../resources/notebook.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|Stream|**TODO: Add Description**|
|contentUrl|String|**TODO: Add Description**|
|createdByAppId|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|level|Int32|**TODO: Add Description**|
|links|[pageLinks](../resources/pagelinks.md)|**TODO: Add Description**|
|order|Int32|**TODO: Add Description**|
|self|String|**TODO: Add Description** Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|
|title|String|**TODO: Add Description**|
|userTags|String collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|parentNotebook|[notebook](../resources/notebook.md)|**TODO: Add Description**|
|parentSection|[onenoteSection](../resources/onenotesection.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onenotePage",
  "baseType": "microsoft.graph.onenoteEntitySchemaObjectModel",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenotePage",
  "id": "String (identifier)",
  "self": "String",
  "createdDateTime": "String (timestamp)",
  "title": "String",
  "createdByAppId": "String",
  "links": {
    "@odata.type": "microsoft.graph.pageLinks"
  },
  "contentUrl": "String",
  "content": "Stream",
  "lastModifiedDateTime": "String (timestamp)",
  "level": "Integer",
  "order": "Integer",
  "userTags": [
    "String"
  ]
}
```

