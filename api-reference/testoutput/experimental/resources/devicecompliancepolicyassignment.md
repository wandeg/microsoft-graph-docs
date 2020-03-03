---
title: "deviceCompliancePolicyAssignment resource type"
description: "Device compliance policy assignment."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# deviceCompliancePolicyAssignment resource type

Device compliance policy assignment.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceCompliancePolicyAssignment](../api/devicecompliancepolicyassignment-get.md)|[deviceCompliancePolicyAssignment](../resources/deviceCompliancePolicyAssignment.md)|Read properties and relationships of the [deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md) object.|
|[Delete deviceCompliancePolicyAssignment](../api/devicecompliancepolicyassignment-delete.md)|None|Deletes a [deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md).|
|[Update deviceCompliancePolicyAssignment](../api/devicecompliancepolicyassignment-update.md)|[deviceCompliancePolicyAssignment](../resources/deviceCompliancePolicyAssignment.md)|Update the properties of a [deviceCompliancePolicyAssignment](../resources/devicecompliancepolicyassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|source|Enumeration|The assignment source for the device compliance policy, direct or parcel/policySet. Possible values are: `direct`, `policySets`.|
|sourceId|String|The identifier of the source of the assignment.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-apps-deviceAndAppManagementAssignmentTarget.md)|Target for the compliance policy assignment.|

## Relationships
None

## JSON Representation
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
  },
  "source": "String",
  "sourceId": "String"
}
```

