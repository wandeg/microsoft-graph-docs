---
title: "sideLoadingKey resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# sideLoadingKey resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get sideLoadingKey](../api/sideloadingkey-get.md)|[sideLoadingKey](../resources/sideloadingkey.md)|Read properties and relationships of the [sideLoadingKey](../resources/sideloadingkey.md) object.|
|[Update sideLoadingKey](../api/sideloadingkey-update.md)|[sideLoadingKey](../resources/sideloadingkey.md)|Update the properties of a [sideLoadingKey](../resources/sideloadingkey.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastUpdatedDateTime|String||
|totalActivation|Int32||
|value|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sideLoadingKey",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "String (identifier)",
  "value": "String",
  "displayName": "String",
  "description": "String",
  "totalActivation": 1024,
  "lastUpdatedDateTime": "String"
}
```

