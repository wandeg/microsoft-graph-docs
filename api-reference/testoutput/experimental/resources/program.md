---
title: "program resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# program resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List programs](../api/program-list.md)|[program](../resources/program.md) collection|List properties and relationships of the [program](../resources/program.md) objects.|
|[Get program](../api/program-get.md)|[program](../resources/program.md)|Read properties and relationships of the [program](../resources/program.md) object.|
|[Create program](../api/program-post-programs.md)|[program](../resources/program.md)|Create a new [program](../resources/program.md) object.|
|[Delete program](../api/program-delete.md)|None|Deletes a [program](../resources/program.md).|
|[Update program](../api/program-update.md)|[program](../resources/program.md)|Update the properties of a [program](../resources/program.md) object.|
|[List controls](../api/program-list-controls.md)|[programControl](../resources/programcontrol.md) collection|Get the programControls from the controls navigation property.|
|[Add controls](../api/program-post-controls.md)|[programControl](../resources/programcontrol.md)|Add controls by posting to the controls collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|controls|[programControl](../resources/programcontrol.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.program",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.program",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```

