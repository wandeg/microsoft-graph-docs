---
title: "programControlType resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# programControlType resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List programControlTypes](../api/programcontroltype-list.md)|[programControlType](../resources/programcontroltype.md) collection|List properties and relationships of the [programControlType](../resources/programcontroltype.md) objects.|
|[Get programControlType](../api/programcontroltype-get.md)|[programControlType](../resources/programcontroltype.md)|Read properties and relationships of the [programControlType](../resources/programcontroltype.md) object.|
|[Create programControlType](../api/programcontroltype-post-programcontroltypes.md)|[programControlType](../resources/programcontroltype.md)|Create a new [programControlType](../resources/programcontroltype.md) object.|
|[Delete programControlType](../api/programcontroltype-delete.md)|None|Deletes a [programControlType](../resources/programcontroltype.md).|
|[Update programControlType](../api/programcontroltype-update.md)|[programControlType](../resources/programcontroltype.md)|Update the properties of a [programControlType](../resources/programcontroltype.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|controlTypeGroupId|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.programControlType",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.programControlType",
  "id": "String (identifier)",
  "controlTypeGroupId": "String",
  "displayName": "String"
}
```

