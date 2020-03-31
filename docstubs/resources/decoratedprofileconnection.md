---
title: "DecoratedProfileConnection resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# DecoratedProfileConnection resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List DecoratedProfileConnections](../api/decoratedprofileconnection-list.md)|[DecoratedProfileConnection](../resources/decoratedprofileconnection.md) collection|List properties and relationships of the [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) objects.|
|[Get DecoratedProfileConnection](../api/decoratedprofileconnection-get.md)|[DecoratedProfileConnection](../resources/decoratedprofileconnection.md)|Read properties and relationships of the [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) object.|
|[Create DecoratedProfileConnection](../api/decoratedprofileconnection-post-decoratedprofileconnections.md)|[DecoratedProfileConnection](../resources/decoratedprofileconnection.md)|Create a new [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) object.|
|[Delete DecoratedProfileConnection](../api/decoratedprofileconnection-delete.md)|None|Deletes a [DecoratedProfileConnection](../resources/decoratedprofileconnection.md).|
|[Update DecoratedProfileConnection](../api/decoratedprofileconnection-update.md)|[DecoratedProfileConnection](../resources/decoratedprofileconnection.md)|Update the properties of a [DecoratedProfileConnection](../resources/decoratedprofileconnection.md) object.|
|[viewer](../api/decoratedprofileconnection-viewer.md)|[DecoratedProfileConnection](../resources/decoratedprofileconnection.md) collection||
|[Get DecoratedProfile](../api/decoratedprofile-get.md)|[DecoratedProfile](../resources/decoratedprofile.md)|Read properties and relationships of the [DecoratedProfile](../resources/decoratedprofile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|relevanceScore|Double||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|profile|[DecoratedProfile](../resources/decoratedprofile.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.DecoratedProfileConnection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.DecoratedProfileConnection",
  "id": "String (identifier)",
  "relevanceScore": "Double"
}
```

