---
title: "DecoratedProfileSearchResult resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# DecoratedProfileSearchResult resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[batchQuery](../api/decoratedprofilesearchresult-batchquery.md)|[DecoratedProfileSearchResult](../resources/decoratedprofilesearchresult.md) collection|**TODO: Add Description**|
|[List profiles](../api/decoratedprofilesearchresult-list-profiles.md)|[DecoratedProfile](../resources/decoratedprofile.md) collection|Get the DecoratedProfiles from the profiles navigation property.|
|[Create profiles](../api/decoratedprofilesearchresult-post-profiles.md)|[DecoratedProfile](../resources/decoratedprofile.md)|Create a new profiles object.|
|[Delete profiles](../api/decoratedprofilesearchresult-delete-profiles.md)|None|Delete a [DecoratedProfile](../resources/decoratedprofile.md) object.|
|[Update profiles](../api/decoratedprofilesearchresult-update-profiles.md)|[DecoratedProfile](../resources/decoratedprofile.md)|Update the properties of a profiles object.|
|[Get profiles](../api/decoratedprofilesearchresult-get-decoratedprofile.md)|[DecoratedProfile](../resources/decoratedprofile.md)|Read the properties and relationships of a [DecoratedProfile](../resources/decoratedprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|exactMatch|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|query|[DecoratedProfileSearchQuery](../resources/decoratedprofilesearchquery.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|profiles|[DecoratedProfile](../resources/decoratedprofile.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.DecoratedProfileSearchQuery"
  },
  "exactMatch": "Boolean"
}
```

