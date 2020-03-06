---
title: "policySetAssignment resource type"
description: "A class containing the properties used for PolicySet Assignment."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# policySetAssignment resource type


Namespace: microsoft.graph

A class containing the properties used for PolicySet Assignment.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get policySetAssignment](../api/policysetassignment-get.md)|[policySetAssignment](../resources/policysetassignment.md)|Read properties and relationships of the [policySetAssignment](../resources/policysetassignment.md) object.|
|[Update policySetAssignment](../api/policysetassignment-update.md)|[policySetAssignment](../resources/policysetassignment.md)|Update the properties of a [policySetAssignment](../resources/policysetassignment.md) object.|
|[List assignments](../api/policyset-list-assignments.md)|[policySetAssignment](../resources/policysetassignment.md) collection|Get the policySetAssignments from the assignments navigation property.|
|[Add assignments](../api/policyset-post-assignments.md)|[policySetAssignment](../resources/policysetassignment.md)|Add assignments by posting to the assignments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Last modified time of the PolicySetAssignment.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|The target group of PolicySetAssignment|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySetAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

