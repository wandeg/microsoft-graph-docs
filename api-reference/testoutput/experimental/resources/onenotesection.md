---
title: "onenoteSection resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# onenoteSection resource type




Inherits from [onenoteEntityHierarchyModel](../resources/onenoteEntityHierarchyModel.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get onenoteSection](../api/onenotesection-get.md)|[onenoteSection](../resources/onenoteSection.md)|Read properties and relationships of the [onenoteSection](../resources/onenotesection.md) object.|
|[Delete onenoteSection](../api/onenotesection-delete.md)|None|Deletes a [onenoteSection](../resources/onenotesection.md).|
|[Update onenoteSection](../api/onenotesection-update.md)|[onenoteSection](../resources/onenoteSection.md)|Update the properties of a [onenoteSection](../resources/onenotesection.md) object.|
|[copyToNotebook](../api/onenotesection-copytonotebook.md)|[onenoteOperation](../resources/onenoteOperation.md)||
|[copyToSectionGroup](../api/onenotesection-copytosectiongroup.md)|[onenoteOperation](../resources/onenoteOperation.md)||
|[Get notebook](../api/notebook-get.md)|[notebook](../resources/notebook.md)|Read properties and relationships of the [notebook](../resources/notebook.md) object.|
|[Get sectionGroup](../api/sectiongroup-get.md)|[sectionGroup](../resources/sectionGroup.md)|Read properties and relationships of the [sectionGroup](../resources/sectiongroup.md) object.|
|[List pages](../api/onenotesection-list-pages.md)|[onenotePage](../resources/onenotePage.md) collection|Get the onenotePages from the pages navigation property.|
|[Add pages](../api/onenotesection-post-pages.md)|[onenotePage](../resources/onenotePage.md)|Add pages by posting to the pages collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identitySet.md)| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteEntityHierarchyModel.md)|
|createdDateTime|DateTimeOffset| Inherited from [onenoteEntitySchemaObjectModel](../resources/onenoteEntitySchemaObjectModel.md)|
|displayName|String| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteEntityHierarchyModel.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean||
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteEntityHierarchyModel.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [onenoteEntityHierarchyModel](../resources/onenoteEntityHierarchyModel.md)|
|links|[sectionLinks](../resources/sectionLinks.md)||
|pagesUrl|String||
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteEntityBaseModel.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|pages|[onenotePage](../resources/onenotePage.md) collection||
|parentNotebook|[notebook](../resources/notebook.md)||
|parentSectionGroup|[sectionGroup](../resources/sectionGroup.md)||

## JSON Representation
Here is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "isDefault": true,
  "links": {
    "@odata.type": "microsoft.graph.sectionLinks"
  },
  "pagesUrl": "String"
}
```

