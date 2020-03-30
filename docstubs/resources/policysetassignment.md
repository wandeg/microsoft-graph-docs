---
title: "policySetAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# policySetAssignment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get policySetAssignment](../api/policysetassignment-get.md)|[policySetAssignment](../resources/policysetassignment.md)|Read properties and relationships of the [policySetAssignment](../resources/policysetassignment.md) object.|
|[Update policySetAssignment](../api/policysetassignment-update.md)|[policySetAssignment](../resources/policysetassignment.md)|Update the properties of a [policySetAssignment](../resources/policysetassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)||

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

