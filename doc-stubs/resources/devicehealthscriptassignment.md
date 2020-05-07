---
title: "deviceHealthScriptAssignment resource type"
description: "Contains properties used to assign a device management script to a group."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceHealthScriptAssignment resource type


Namespace: microsoft.graph

Contains properties used to assign a device management script to a group.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Key of the device health script assignment entity. This property is read-only.|
|runRemediationScript|Boolean|Determine whether we want to run detection script only or run both detection script and remediation script|
|runSchedule|[runSchedule](../resources/runschedule.md)|Script run schedule for the target group|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|The Azure Active Directory group we are targeting the script to|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.management.services.api.deviceHealthScriptAssignment",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.deviceHealthScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.management.services.api.deviceAndAppManagementAssignmentTarget"
  },
  "runRemediationScript": "Boolean",
  "runSchedule": {
    "@odata.type": "microsoft.management.services.api.runSchedule"
  }
}
```

