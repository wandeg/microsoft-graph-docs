---
title: "DecoratedProfileSearchResult resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# DecoratedProfileSearchResult resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List DecoratedProfileSearchResults](../api/decoratedprofilesearchresult-list.md)|[DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) collection|List properties and relationships of the [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) objects.|
|[Get DecoratedProfileSearchResult](../api/decoratedprofilesearchresult-get.md)|[DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md)|Read properties and relationships of the [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) object.|
|[Create DecoratedProfileSearchResult](../api/decoratedprofilesearchresult-post-decoratedprofilesearchresults.md)|[DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md)|Create a new [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) object.|
|[Delete DecoratedProfileSearchResult](../api/decoratedprofilesearchresult-delete.md)|None|Deletes a [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md).|
|[Update DecoratedProfileSearchResult](../api/decoratedprofilesearchresult-update.md)|[DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md)|Update the properties of a [DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) object.|
|[batchQuery](../api/decoratedprofilesearchresult-batchquery.md)|[DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) collection||
|[List profiles](../api/decoratedprofilesearchresult-list-profiles.md)|[DecoratedProfile](../resources/decoratedprofile.md) collection|Get the DecoratedProfiles from the profiles navigation property.|
|[Add profiles](../api/decoratedprofilesearchresult-post-profiles.md)|[DecoratedProfile](../resources/decoratedprofile.md)|Add profiles by posting to the profiles collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|exactMatch|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|query|[DecoratedProfileSearchQuery](../resources/decoratedprofilesearchquery.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|profiles|[DecoratedProfile](../resources/decoratedprofile.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.DecoratedProfileSearchResult",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.DecoratedProfileSearchResult",
  "id": "String (identifier)",
  "query": {
    "@odata.type": "microsoft.graph.DecoratedProfileSearchQuery",
    "email": "String",
    "keywords": "String"
  },
  "exactMatch": true
}
```

