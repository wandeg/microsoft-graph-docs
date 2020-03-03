---
title: "onenotePage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# onenotePage resource type




Inherits from [onenoteEntitySchemaObjectModel](../resources/onenoteEntitySchemaObjectModel.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get onenotePage](../api/onenotepage-get.md)|[onenotePage](../resources/onenotePage.md)|Read properties and relationships of the [onenotePage](../resources/onenotepage.md) object.|
|[Delete onenotePage](../api/onenotepage-delete.md)|None|Deletes a [onenotePage](../resources/onenotepage.md).|
|[Update onenotePage](../api/onenotepage-update.md)|[onenotePage](../resources/onenotePage.md)|Update the properties of a [onenotePage](../resources/onenotepage.md) object.|
|[onenotePatchContent](../api/onenotepage-onenotepatchcontent.md)|None||
|[preview](../api/onenotepage-preview.md)|[onenotePagePreview](../resources/onenotePagePreview.md)||
|[copyToSection](../api/onenotepage-copytosection.md)|[onenoteOperation](../resources/onenoteOperation.md)||
|[Get onenoteSection](../api/onenotesection-get.md)|[onenoteSection](../resources/onenoteSection.md)|Read properties and relationships of the [onenoteSection](../resources/onenotesection.md) object.|
|[Get notebook](../api/notebook-get.md)|[notebook](../resources/notebook.md)|Read properties and relationships of the [notebook](../resources/notebook.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|Stream||
|contentUrl|String||
|createdByAppId|String||
|createdDateTime|DateTimeOffset| Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteEntitySchemaObjectModel.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|level|Int32||
|links|[pageLinks](../resources/pageLinks.md)||
|order|Int32||
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteEntityBaseModel.md)|
|title|String||
|userTags|String collection||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|parentNotebook|[notebook](../resources/notebook.md)||
|parentSection|[onenoteSection](../resources/onenoteSection.md)||

## JSON Representation
Here is a JSON representation of the resource.
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
  "level": 1024,
  "order": 1024,
  "userTags": [
    "String"
  ]
}
```

