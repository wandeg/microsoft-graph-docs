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
|[List policySetAssignments](../api/policysetassignment-list.md)|[policySetAssignment](../resources/policysetassignment.md) collection|List properties and relationships of the [policySetAssignment](../resources/policysetassignment.md) objects.|
|[Get policySetAssignment](../api/policysetassignment-get.md)|[policySetAssignment](../resources/policysetassignment.md)|Read properties and relationships of the [policySetAssignment](../resources/policysetassignment.md) object.|
|[Create policySetAssignment](../api/policysetassignment-create.md)|[policySetAssignment](../resources/policysetassignment.md)|Create a new [policySetAssignment](../resources/policysetassignment.md) object.|
|[Delete policySetAssignment](../api/policysetassignment-delete.md)|None|Deletes a [policySetAssignment](../resources/policysetassignment.md).|
|[Update policySetAssignment](../api/policysetassignment-update.md)|[policySetAssignment](../resources/policysetassignment.md)|Update the properties of a [policySetAssignment](../resources/policysetassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Last modified time of the PolicySetAssignment.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-apps-deviceandappmanagementassignmenttarget.md)|The target group of PolicySetAssignment|

## Relationships
None

## JSON Representation
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

