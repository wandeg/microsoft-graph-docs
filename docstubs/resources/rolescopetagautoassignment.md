---
title: "roleScopeTagAutoAssignment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# roleScopeTagAutoAssignment resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get roleScopeTagAutoAssignment](../api/rolescopetagautoassignment-get.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md)|Read properties and relationships of the [roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) object.|
|[Update roleScopeTagAutoAssignment](../api/rolescopetagautoassignment-update.md)|[roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md)|Update the properties of a [roleScopeTagAutoAssignment](../resources/rolescopetagautoassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.roleScopeTagAutoAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

