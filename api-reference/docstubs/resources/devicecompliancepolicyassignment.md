---
title: "deviceCompliancePolicyAssignment resource type"
description: "Device compliance policy assignment."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# deviceCompliancePolicyAssignment resource type


Namespace: microsoft.graph

Device compliance policy assignment.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceCompliancePolicyAssignment](../api/devicecompliancepolicyassignment-get.md)|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md)|Read properties and relationships of a [deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md) object.|
|[Update deviceCompliancePolicyAssignment](../api/devicecompliancepolicyassignment-update.md)|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md)|Update the properties of a [deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md) object.|
|[List assignments](../api/devicecompliancepolicy-list-assignments.md)|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md) collection|Get the deviceCompliancePolicyAssignments from the assignments navigation property.|
|[Create assignments](../api/devicecompliancepolicy-post-assignments.md)|[deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md)|Create a new assignments object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|Target for the compliance policy assignment.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

