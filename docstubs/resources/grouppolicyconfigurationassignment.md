---
title: "groupPolicyConfigurationAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyConfigurationAssignment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyConfigurationAssignment](../api/grouppolicyconfigurationassignment-get.md)|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md)|Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) object.|
|[Update groupPolicyConfigurationAssignment](../api/grouppolicyconfigurationassignment-update.md)|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md)|Update the properties of a [groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) object.|

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
  "@odata.type": "microsoft.graph.groupPolicyConfigurationAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

