---
title: "deviceCategory resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceCategory resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceCategory](../api/devicecategory-get.md)|[deviceCategory](../resources/devicecategory.md)|Read properties and relationships of the [deviceCategory](../resources/devicecategory.md) object.|
|[Update deviceCategory](../api/devicecategory-update.md)|[deviceCategory](../resources/devicecategory.md)|Update the properties of a [deviceCategory](../resources/devicecategory.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|roleScopeTagIds|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```

