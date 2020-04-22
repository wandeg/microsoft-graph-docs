---
title: "program resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# program resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List programs](../api/program-list.md)|[program](../resources/program.md) collection|Get a list of the [program](../resources/program.md) objects and their properties.|
|[Get program](../api/program-get.md)|[program](../resources/program.md)|Read properties and relationships of a [program](../resources/program.md) object.|
|[Create program](../api/program-post-programs.md)|[program](../resources/program.md)|Create a new [program](../resources/program.md) object.|
|[Delete program](../api/program-delete.md)|None|Deletes a [program](../resources/program.md).|
|[Update program](../api/program-update.md)|[program](../resources/program.md)|Update the properties of a [program](../resources/program.md) object.|
|[List controls](../api/program-list-controls.md)|[programControl](../resources/programcontrol.md) collection|Get the programControls from the controls navigation property.|
|[Create controls](../api/program-post-controls.md)|[programControl](../resources/programcontrol.md)|Create a new controls object.|
|[Delete controls](../api/program-delete-controls.md)|None|Delete a controls object.|
|[Update controls](../api/program-update-controls.md)|[programControl](../resources/programcontrol.md)|Update the properties of a controls object.|
|[Get programControl](../api/programcontrol-get.md)|[programControl](../resources/programcontrol.md)|Read properties and relationships of a [programControl](../resources/programcontrol.md) object.|
|[List program](../api/programcontrol-list-program.md)|[program](../resources/program.md) collection|Get the programs from the program navigation property.|
|[Create program](../api/programcontrol-post-program.md)|[program](../resources/program.md)|Create a new program object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|controls|[programControl](../resources/programcontrol.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.program",
  "baseType": "",
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

