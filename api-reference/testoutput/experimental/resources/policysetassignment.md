---
title: "policySetAssignment resource type"
description: "A class containing the properties used for PolicySet Assignment."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# policySetAssignment resource type

A class containing the properties used for PolicySet Assignment.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get policySetAssignment](../api/policysetassignment-get.md)|[policySetAssignment](../resources/policySetAssignment.md)|Read properties and relationships of the [policySetAssignment](../resources/policysetassignment.md) object.|
|[Delete policySetAssignment](../api/policysetassignment-delete.md)|None|Deletes a [policySetAssignment](../resources/policysetassignment.md).|
|[Update policySetAssignment](../api/policysetassignment-update.md)|[policySetAssignment](../resources/policySetAssignment.md)|Update the properties of a [policySetAssignment](../resources/policysetassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|Last modified time of the PolicySetAssignment.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-apps-deviceAndAppManagementAssignmentTarget.md)|The target group of PolicySetAssignment|

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

