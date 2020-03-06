---
title: "deviceHealthScriptAssignment resource type"
description: "Contains properties used to assign a device management script to a group."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceHealthScriptAssignment resource type


Namespace: microsoft.graph

Contains properties used to assign a device management script to a group.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceHealthScriptAssignment](../api/devicehealthscriptassignment-get.md)|[deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md)|Read properties and relationships of the [deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) object.|
|[Update deviceHealthScriptAssignment](../api/devicehealthscriptassignment-update.md)|[deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md)|Update the properties of a [deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) object.|
|[List assignments](../api/devicehealthscript-list-assignments.md)|[deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md) collection|Get the deviceHealthScriptAssignments from the assignments navigation property.|
|[Add assignments](../api/devicehealthscript-post-assignments.md)|[deviceHealthScriptAssignment](../resources/devicehealthscriptassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|runRemediationScript|Boolean|Determine whether we want to run detection script only or run both detection script and remediation script|
|runSchedule|[runSchedule](../resources/runschedule.md)|Script run schedule for the target group|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|The Azure Active Directory group we are targeting the script to|

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

