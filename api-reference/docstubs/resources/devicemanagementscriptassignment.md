---
title: "deviceManagementScriptAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceManagementScriptAssignment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceManagementScriptAssignment](../api/devicemanagementscriptassignment-get.md)|[deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md)|Read properties and relationships of the [deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) object.|
|[Update deviceManagementScriptAssignment](../api/devicemanagementscriptassignment-update.md)|[deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md)|Update the properties of a [deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

