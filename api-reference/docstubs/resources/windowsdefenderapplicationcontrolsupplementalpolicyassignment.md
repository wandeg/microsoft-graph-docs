---
title: "windowsDefenderApplicationControlSupplementalPolicyAssignment resource type"
description: "A class containing the properties used for assignment of a WindowsDefenderApplicationControl supplemental policy to a group."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsDefenderApplicationControlSupplementalPolicyAssignment resource type


Namespace: microsoft.graph

A class containing the properties used for assignment of a WindowsDefenderApplicationControl supplemental policy to a group.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get windowsDefenderApplicationControlSupplementalPolicyAssignment](../api/windowsdefenderapplicationcontrolsupplementalpolicyassignment-get.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Read the properties and relationships of a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.|
|[Update windowsDefenderApplicationControlSupplementalPolicyAssignment](../api/windowsdefenderapplicationcontrolsupplementalpolicyassignment-update.md)|[windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/windowsdefenderapplicationcontrolsupplementalpolicyassignment.md)|Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyAssignment](../resources/windowsdefenderapplicationcontrolsupplementalpolicyassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|The target group assignment defined by the admin.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

