---
title: "allowedDataLocation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# allowedDataLocation resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List allowedDataLocations](../api/alloweddatalocation-list.md)|[allowedDataLocation](../resources/alloweddatalocation.md) collection|List properties and relationships of the [allowedDataLocation](../resources/alloweddatalocation.md) objects.|
|[Get allowedDataLocation](../api/alloweddatalocation-get.md)|[allowedDataLocation](../resources/alloweddatalocation.md)|Read properties and relationships of the [allowedDataLocation](../resources/alloweddatalocation.md) object.|
|[Create allowedDataLocation](../api/alloweddatalocation-post-alloweddatalocations.md)|[allowedDataLocation](../resources/alloweddatalocation.md)|Create a new [allowedDataLocation](../resources/alloweddatalocation.md) object.|
|[Delete allowedDataLocation](../api/alloweddatalocation-delete.md)|None|Deletes a [allowedDataLocation](../resources/alloweddatalocation.md).|
|[Update allowedDataLocation](../api/alloweddatalocation-update.md)|[allowedDataLocation](../resources/alloweddatalocation.md)|Update the properties of a [allowedDataLocation](../resources/alloweddatalocation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appId|String||
|domain|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean||
|location|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.allowedDataLocation",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.allowedDataLocation",
  "id": "String (identifier)",
  "appId": "String",
  "location": "String",
  "isDefault": true,
  "domain": "String"
}
```

