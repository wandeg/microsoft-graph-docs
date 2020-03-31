---
title: "userConfiguration resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userConfiguration resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userConfiguration](../api/userconfiguration-get.md)|[userConfiguration](../resources/userconfiguration.md)|Read properties and relationships of the [userConfiguration](../resources/userconfiguration.md) object.|
|[Update userConfiguration](../api/userconfiguration-update.md)|[userConfiguration](../resources/userconfiguration.md)|Update the properties of a [userConfiguration](../resources/userconfiguration.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|binaryData|Binary||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userConfiguration",
  "id": "String (identifier)",
  "binaryData": "binary"
}
```

