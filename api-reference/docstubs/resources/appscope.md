---
title: "appScope resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# appScope resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get appScope](../api/appscope-get.md)|[appScope](../resources/appscope.md)|Read properties and relationships of the [appScope](../resources/appscope.md) object.|
|[Update appScope](../api/appscope-update.md)|[appScope](../resources/appscope.md)|Update the properties of a [appScope](../resources/appscope.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|type|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appScope",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appScope",
  "id": "String (identifier)",
  "type": "String",
  "displayName": "String"
}
```

