---
title: "deviceHealthScriptAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceHealthScriptAssignment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceHealthScriptAssignment](../api/devicehealthscriptassignment-get.md)|[deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md)|Read properties and relationships of the [deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) object.|
|[Update deviceHealthScriptAssignment](../api/devicehealthscriptassignment-update.md)|[deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md)|Update the properties of a [deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|runRemediationScript|Boolean||
|runSchedule|[runSchedule](../resources/runschedule.md)||
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "runRemediationScript": true,
  "runSchedule": {
    "@odata.type": "microsoft.graph.runSchedule"
  }
}
```

