---
title: "groupPolicyConfigurationAssignment resource type"
description: "The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPolicyConfigurationAssignment resource type


Namespace: microsoft.graph

The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get groupPolicyConfigurationAssignment](../api/grouppolicyconfigurationassignment-get.md)|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md)|Read the properties and relationships of a [groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) object.|
|[Update groupPolicyConfigurationAssignment](../api/grouppolicyconfigurationassignment-update.md)|[groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md)|Update the properties of a [groupPolicyConfigurationAssignment](../resources/grouppolicyconfigurationassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|The type of groups targeted the group policy configuration.|

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

