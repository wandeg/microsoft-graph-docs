---
title: "groupPolicyConfigurationAssignment resource type"
description: "The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPolicyConfigurationAssignment resource type


Namespace: microsoft.graph

The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupPolicyConfigurationAssignments](../api/grouppolicyconfigurationassignment-list.md)|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) collection|List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) objects.|
|[Get groupPolicyConfigurationAssignment](../api/grouppolicyconfigurationassignment-get.md)|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md)|Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) object.|
|[Create groupPolicyConfigurationAssignment](../api/grouppolicyconfigurationassignment-create.md)|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md)|Create a new [groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) object.|
|[Delete groupPolicyConfigurationAssignment](../api/grouppolicyconfigurationassignment-delete.md)|None|Deletes a [groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md).|
|[Update groupPolicyConfigurationAssignment](../api/grouppolicyconfigurationassignment-update.md)|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md)|Update the properties of a [groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-apps-deviceandappmanagementassignmenttarget.md)|The type of groups targeted the group policy configuration.|

## Relationships
None

## JSON Representation
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

